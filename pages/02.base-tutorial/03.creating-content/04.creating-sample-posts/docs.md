---
title: 'Creating Sample Posts'
media_order: add-sample-page.png
taxonomy:
    category:
        - docs
---

We should add several more posts to our blog so we can see how it will look when it is all put together.

You can make your own posts if you like, but I have provided several sample posts that you can use as well. You can follow along on this page to make each of these posts.

!!!! A sample repository is in the works where you will also be able to download these pages and upload them to your website using the file manager, instead.

## The Posts

Remember for each of these to use the _Item_ template, to not make the page visible, and to set the parent page to _(blog) Blog_, as below.

! If you accidentally make a page visible (you will notice because there will be a dropdown menu for Blog on your website), you can change it in the _Advanced_ tab under Overrides. Find _Visible_ and click _Disabled_.

![The Add Page dialog box. Page Title: Sample Title. Folder Name: sample-title. Parent Page: --> (blog) Blog. Page Template: Item. Visible: No.](add-sample-page.png)

The following details will be provided for each page:

- Content Tab
  - Title
  - Content (for the Markdown editor)
  - Page Media
- Options Tab
  - Tags (both a list of tags and the yaml text that would go into the Frontmatter)
- Blog Item Tab
  - Hero Classes
  - Hero Image
- Frontmatter

The Frontmatter section will provide the yaml text that would go into the Frontmatter if you are using Expert mode. If you choose to use Expert mode, all you have to do is upload any images specified to the Page Media, copy the Content into the Markdown editor, and copy the Frontmatter.

### 1. Media in Markdown

#### Cotent

Title: `CLIP: Media in Markdown`

Content:

```md
CLIP: As mentioned in the [tutorial](http://ds-tutorials.oucreate.com/base-tutorial/content/media), there are two ways to add images to your pages. The tutorial walks you through uploading an image and then setting it as the "hero image" used by the page template. It also provides a brief description of adding images within the content. In this post we will demonstrate adding an image within the content.

![An image from the total solar eclipse of 2017, taken from Casper Wyoming some time before totality.](eclipse-2017.png)

Total Solar Eclipse 2017, Wyoming by [Wendy Acker](https://www.flickr.com/people/theodwynn/), [CC BY-NS-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

The Markdown for adding an image looks like ![alt text](image url). If the media has been added to the page that is using it (by uploading it the same way you would before setting it as the hero image), the url can simply be the name of the image, like this: ![alt text](image.png) or ![alt text](./image.png). If you are using an image located elsewhere on your website you will need to provide either the full url or the relative url (for example, image.png and ./image.png are relative urls). I strongly recommend uploading the images you use directly to the page (or to a seperate folder on your website). An image posted elsewhere on the internet might be taken down at some point, leaving you with a broken image link.

! Please note the alt text (or alternative text) section in the Markdown for adding an image. It is extremely important to provide good alt text for any image you add to your content. If the image is ever removed, the broken link will display the alt text instead, allowing users to at least know what used to be there. More importantly, visually impaired users can benefit from good alt text, since they may not be able to make use of the image itself.

Note that for this post, there is only one piece of media added. The blog page displays the image on the summary, but the post page does not show the image as a header/hero. If you do not want to use a header image, but still want to show an image with your post, this is an excellent way to do so.
```

Page Media:
- _Total Solar Eclipse 2017, Wyoming_ **as** _eclipse-2017.png_

#### Options

Tags:
- tutorial
- markdown
- astronomy

#### Blog Item

Hero Classes: _none_

Hero Image: _none_

#### Frontmatter

```yaml
CLIP: title: 'Media in Markdown'
media_order: eclipse-2017.png
taxonomy:
    tag:
        - tutorial
        - markdown
        - astronomy
feed:
    limit: 10
```

### 2. File Naming Conventions

#### Content

Title: `CLIP: File Naming Convenetions`

Content:
```md
CLIP: I have always had a difficult time naming things - whether it is an essay for a class, a character in a story, or even a simple file or folder on my computer. There are so many possible names, and it can feel overwhelming trying to make sure I choose the best name.

===

Fortunately, there are three principles for naming files that can make coming up with the right name considerably easier.

## Machine Readable

Files are stored on computers, so they should be named in ways that the computer can understand.

- Avoid spaces, punctuation, and accented characters.
- Do not make file names case-sensitive - that is, do not name one file _my-file.txt_ and another one _my-File.txt_.
- Use delimiters like hypens "-" and underscores "\_" deliberately. Or just use them to make sure your eyes don't bleed.

Avoiding spaces might seem difficult, but there are two excellent ways to have effective multi-word titles without spaces.
- Use hyphens or underscores to separate words: _my-file.txt_ or _my\_file.txt_.
- Use camel case - every word after the first word is capitalized: myFile.txt

## Human Readable

There is really only one primary requirement for a file to be human readable: The name should provide information about the file contents, the more specific (without being ridiculous long) the better.

If you are writing the first draft of a research paper, for example, the most uninformative name you could choose would be something like _untitled.txt_. Only slightly better are names like _paper.txt_ or _first-draft.txt_. The best name would include some kind of version information, perhaps the date you wrote it, as well as information about the actual contents of the paper that would differentiate it from any other paper you have written or might write in the future. So if you started work on this particular draft on January 1 2020 and the paper is about why libraries are great, an excellent title might be _why-libraries-are-great_2020-01-01.txt_ or _2020-01-01_why-libraries-are-great.txt_.

## Using Default Ordering

Mostly this comes down to letting the system order your files logically based on numbers - for example, sorting your essay drafts based on date. There are a lot of different ways you might do this depending on what exactly you want, but there are two things to keep in mind when using numbers and dates to order files.

1. **Pad numbers with 0.** 3 will generally be listed after 20, because 3 comes after 2. However, 03 will always come before 20. If you are using numbers, make sure to use the same number of digits for each number, adding 0 as necessary.
2. **Use they year-month-day (YYYY-MM-DD) format for dates.** This will allow the system to sort your files accurately based on the date. Imagine three files created on March 10 2018, January 1 2019, and December 23 2019. Using a format like MM-DD-YYYY, trying to sort the files in descending (most recent) order would yield: _12-23-2019_words.txt_, _03-10-2018_words.txt_, _01-01-2019_words.txt_. Semantically, this order makes little sense - a file written in 2018 is listed between two files written in 2019. Using YYYY-MM-DD would instead order the files as: _2019-12-23_words.txt_, _2019-01-01_words.txt_, _2018-03-10_words.txt_. This is much more logical and convenient.

## The Carpentries

There are many advantages to following file naming conventions or best practices. For more information on these advantages, as well as the practices themselves, read the Data Carpentry lesson [File Organization: Naming](https://datacarpentry.org/rr-organization1/01-file-naming/index.html). The Carpentries teaches foundational coding and data science skills through Data Carpentry, Software Carpentry, and Library Carpentry lessons. Check out their [website](https://carpentries.org/) or take a look at the [schedule](https://libraries.ou.edu/content/software-and-data-carpentry) for workshops offered by OU Libraries.

## Credit

The material for this post comes from the Data Carpentry lesson [File Organization: Naming](https://datacarpentry.org/rr-organization1/01-file-naming/index.html). All lessons are copyright of [The Carpentries](https://carpentries.org/), [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/legalcode).

Photo: Yellowstone by [Wendy Acker](https://www.flickr.com/people/theodwynn/), [CC BY-NS-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
```

Page Media:
- _Yellowstone_ **as** _yellowstone.png_

#### Options

Tags:
- the carpentries
- landscape photo
- yellowstone

#### Blog Item

Hero Classes: `CLIP: title-h1h2 text-light overlay-dark-gradient`

Hero Image: _yellowstone.png_

#### Frontmatter

```yaml
CLIP: title: 'File Naming Conventions'
media_order: yellowstone.png
taxonomy:
    tag:
        - 'the carpentries'
        - 'landscape photo'
        - yellowstone
hero_classes: 'title-h1h2 text-light overlay-dark-gradient'
hero_image: yellowstone.png
feed:
    limit: 10
```

### 3. Telescopes

#### Content

Title: `CLIP: Telescopes`

Content:

```md
CLIP: Did you know you can check out a telescope at Bizzell Memorial Library? 

===

The Orion StarBlast 4.5" reflector telescope is the preferred telescope of the [Library Telescope Program](https://www.astroleague.org/content/library-telescope-program). This program helps public libraries across the U.S. obtain telescopes their patrons can check out. The program advocates for a series of key modifications to make these telescopes library-friendly right out of the box, and libraries not affiliated with the program are still able to purchase the telescopes.

OU Libraries has a rich technology lending program, which now includes astronomy equipment like the telescope. For more information about telescope lending, check out [this guide](http://guides.ou.edu/telescope).

## Photo Credit

The Southern Milky Way, New Zealand by [Wendy Acker](https://www.flickr.com/people/theodwynn/), [CC BY-NS-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
```

Page Media:
- _The Southern Milky Way, New Zealand_ as _milky-way.png_

#### Options

Tags:
- astronomy
- ou libraries

#### Blog Item

Hero Classes: `CLIP: title-h1h2 text-light overlay-dark-gradient`

Hero Image: _milky-way.png_

#### Frontmatter

```yaml
CLIP: title: Telescopes
media_order: milky-way.png
taxonomy:
    tag:
        - astronomy
        - 'ou libraries'
hero_classes: 'title-h1h2 text-light overlay-dark-gradient'
hero_image: milky-way.png
feed:
    limit: 10
```

### 4. Configuring Quark

#### Content

Title: `CLIP: Configuring Quark`

Content: 
```md
CLIP: As of this post, Quark is the default theme for Grav websites. It has a number of configurable options that you may want to check out.

===

To access these options, go to the _Themes_ tab in your admin panel and click on Quark. The most likely options you will be interested in are the grid size and custom logo options.

The grid size determines the maximum width of the frame for your website and by default is set to _Large_. I personally prefer _Extra Large_, as _Large_ creates large swathes of empty space on either side of the blog when I use a large monitor. Try changing the settings and see how that changes your blog.

The custom logo replaces the Grav logo at the top left. You could use a personal or organization logo, or even take a screenshot of your name in a nice font.
```

Page Media: _none_

#### Options

Tags:
- grav
- tutorial

#### Blog Item

Hero Classes: _none_

Hero Image: _none_

#### Frontmatter
```yaml
CLIP: title: 'Configuring Quark'
taxonomy:
    tag:
        - grav
        - tutorial
feed:
    limit: 10
```

### 5. Media Literacy

#### Content

Title: `CLIP: Media Literacy`

Content: 
```md
CLIP: You can't trust everything you see on the internet. But can you trust _anything_ you see on the internet?

===

It can be difficult to know what to believe and what to ignore when anyone could theoretically make up anything. If you care enough about a claim you can, of course, research it thoroughly, but that seems like quite an investment of time, especially when we all encounter so many claims and stories every single day. 

Fortunately, it is possible to do some simple digging to investigate any given claim without having devote very much time at all. The process for this is covered in the two and a half to three hour online curriculum [Check, Please!](https://www.notion.so/Check-Please-Starter-Course-ae34d043575e42828dc2964437ea4eed). Even if you don't have enough time to go through all of it, just working through the first lesson will give you a good introduction to media literacy and becoming an informed consumer.

## Photo Credit

Pancake Rocks, New Zealand by [Wendy Acker](https://www.flickr.com/people/theodwynn/), [CC BY-NS-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
```

Page Media:
- _Pancake Rocks, New Zealand_ **as** _pancake-rocks-nz.png_

#### Options

Tags:
- landscape photo

#### Blog Item

Hero Classes: `CLIP: title-h1h2 text-light overlay-dark-gradient`

Hero Image: _pancake-rocks-nz.png_

#### Frontmatter
```yaml
CLIP: title: 'Media Literacy'
media_order: pancake-rocks-nz.png
taxonomy:
    tag:
        - 'landscape photo'
hero_classes: 'title-h1h2 text-light overlay-dark-gradient'
hero_image: pancake-rocks-nz.png
feed:
    limit: 10
```

### 6. Library Workshops

#### Content

Title: ```CLIP: Library Workshops```

Content: 
```md
CLIP: The University of Oklahoma Libraries offers numerous workshops throughout the year, with topics ranging from knitting to automating repetitive tasks using the programming language R.

===

Whatever your interests (or needs), there are likely at least a few workshops you would find interesting and/or useful. You can check out the [OU Libraries calendar](https://libraries.ou.edu/calendar-node-field-event-date/month) to see what events and workshops are coming up. Make sure to check back regularly to see what new events may have been scheduled.

Don't see a workshop you want? See a workshop you want that isn't offered at a good time? View our [list of on-request workshops](https://libraries.ou.edu/content/university-libraries-request-workshops). For most of these, as long as five people plan to attend we will schedule one for you. The Carpentry workshops are an exception, as they are very long (2 8-hour days). They require a minimum of fifteen participants.

If we have a workshop you are interested in that is not listed as an on-request workshop, or if you don't see a workshop on something that you want to learn, please [contact us](https://libraries.ou.edu/content/contact-us) and let us know! Your feedback can help inform our future directions, and we may be able to direct you to relevant resources, if nothing else.
```

Page Media:
- _Texas Wildflowers_ **as** _texas-wildflowers.png_

#### Options

Tags:
- landscape photo
- ou libraries

#### Blog Item

Hero Classes: ```CLIP: title-h1h2 text-light overlay-dark-gradient```

Hero Image: _texas-wildflowers.png_

#### Frontmatter
```yaml
CLIP: title: 'Library Workshops'
media_order: texas-wildflowers.png
taxonomy:
    tag:
        - 'landscape photo'
        - 'ou libraries'
hero_classes: 'title-h1h2 text-light overlay-dark-gradient'
hero_image: texas-wildflowers.png
feed:
    limit: 10
```

### 7. Fantasy Books

#### Content

Title: ```CLIP: Fantasy Books```

Content: 
```md
CLIP: Books are great! My favorite genre is fantasy, particularly high fantasy - think Lord of the Rings style.

===

## Books

In no particular order, here are some books.

### Lord of the Rings

While not everyone finds it easy to get into _Lord of the Rings_, it definitely deserves a place (or at least a mention) on any fantasy reading list, if only because J. R. R. Tolkein is the father of modern fantasy. _Lord of the Rings_ focuses very heavily on world building, and the languages are particularly well-developed, since Tolkein himself was a linguist. If you find the trilogy is not quite your style, you might still enjoy reading _The Hobbit_.

### Wheel of Time

This fourteen book series was written by Robert Jordan until his death and then continued and completed by Brandon Sanderson (Jordan prepared extensive notes, as he had been diagnosed with a terminal illness). The books are all extremely thick, so this series is a major time commitment. It is also one of my all time favorites with a beautifully developed world, extensive character development, and an epic storyline. It contains mature themes but is remarkably clean.

### Codex Alera

This six book series was written by Jim Butcher, who is also the author of the popular urban fantasy series _The Dresden Files_. I prefer the _Codex Alera_, mostly because it is high fantasy. Both series are a much lighter read than _Lord of the Rings_ or _Wheel of Time_. Fun fact: Apparently the inspiration for _Codex Alera_ came from a heated debate about whether a strong enough premise could carry a book despite a lousy writer, or whether a lousy premise could be made up for by a strong enough writer. The conclusion of this was Butcher agreeing to write a story using two terrible ideas provided to him, which ended up being Lost Roman Legion and Pokemon (Johnson, 2010).

Johnson, B. (2010). _Jim Butcher chats about Pokemon, responsibility, and changes._ Fantasy Literature. http://www.fantasyliterature.com/author-interviews/jim-butcher/

### Harry Potter

This seven book series was written by J. K. Rowling. To be honest, I have a love-hate relationship with this one. It's an incredible and imaginative world, but, given that it began as more of a kids' adventure, there are a lot of plot holes. Also, J. K. Rowling keeps trying to say things about the world, but for my sanity I consider everything from the 1st book to the right before the epilogue is the last book as canon, along with _Tales of Beedle and the Bard_, _Fantastic Beasts and Where to Find Them_ (the book, not the movie), and _Quidditch Through the Ages_. The epilogue falls somewhere between canon and not. Everything from Pottermore or _The Cursed Child_ or elsewhere I consider unequivocally not canon. If you are a person who tends to care about these things, for your own sanity, I recommend doing the same.

### The Deed of Paksenarrion

This trilogy was written by Elizabeth Moon. There is also a sequel trilogy. Moon writes a lot of science fiction, but this represents an extremely successful foray into fantasy writing. _The Deed of Paksenarrion_ is military focused (Paks is a warrior by trade) and is very strong in detail. The story is harsh at places, but I would strongly recommend it!

### Other worthwhile fantasy reads

- _The Name of the Wind_ by Patrick Rothfuss
- Anything by Brandon Sanderson
- The webserial [_The Gods are Bastards_](https://tiraas.net/2014/08/20/book-1-prologue/) by D. D. Webb (high fantasy and western setting, in-progress)
- The weberial [_A Practrical Guide to Evil_](https://practicalguidetoevil.wordpress.com/2015/03/25/prologue/) by ErraticErrata (David Verburg) (in-progress)

```

Page Media:
- _Queenstown Hill, New Zealand_ **as** _queenstown-hill-nz.png_

#### Options

Tags:
- landscape photo
- just for fun

#### Blog Item

Hero Classes: ```CLIP: title-h1h2 text-light overlay-dark-gradient```

Hero Image: _queenstown-hill-nz.png_

#### Frontmatter
```yaml
CLIP: title: 'Fantasy Books'
media_order: queenstown-hill-nz.png
taxonomy:
    tag:
        - 'landscape photo'
        - 'just for fun'
hero_classes: 'title-h1h2 text-light overlay-dark-gradient'
hero_image: queenstown-hill-nz.png
feed:
    limit: 10
```

### 8. Library Resources and Research Help

#### Content

Title: ```CLIP: Library Resources and Research Help```

Content: 
```md
CLIP: If you have looked for a book at OU Libraries, chances are you have used the Discover box at the top of the main library website. Sometimes, however, this is not the most efficient way to find what you are looking for.

===

Oftentimes research requires a bit more specificity in searching. For example, you may need to find articles that fit some particular criteria to be useful for your study or paper. In these cases, a Discover search may be too general. You may find it more helpful to check out our [Databases & E-Reference](https://libraries.ou.edu/eresources), which provides access to a wide variety of databases.

Not sure what database to use? There are so many options that it can easily become overwhelming. For more general article searching, I typically start with Academic Search Primiere, EBSCO, JSTOR, or ProQuest. However, we have other resources available to help you choose. You can start by checking out our [research guides](https://libraries.ou.edu/guides-index) linked to from the library website, or by going to [guides.ou.edu](https://guides.ou.edu/home). Here you can look up the subject you are researching and see what databases we recommend, as well as get information on other potential sources of information or tips for how to find what you need.

For additional research help, visit the Learning Lab on Lower Level One of Bizzell Memorial Library, [contact us](https://libraries.ou.edu/content/contact-us), or contact/schedule an appointment with your subject librarian.
```

Page Media:
- _Wyoming Sunset_ **as** _wyoming-sunset.png_

#### Options

Tags:
- landscape photo
- ou libraries

#### Blog Item

Hero Classes: ```CLIP: title-h1h2 text-light overlay-dark-gradient```

Hero Image: _wyoming-sunset.png_

#### Frontmatter
```yaml
CLIP: title: 'Library Resources and Research Help'
media_order: wyoming-sunset.png
taxonomy:
    tag:
        - 'landscape photo'
        - 'ou libraries'
hero_classes: 'title-h1h2 text-light overlay-dark-gradient'
hero_image: wyoming-sunset.png
feed:
    limit: 10
```

### 9. Parks

#### Content

Title: ```CLIP: Parks```

Content: 
```md
CLIP: I don't love camping, but I do enjoy hiking (in good weather) and enjoying beautiful nature.

===

The top four parks I have visited are Point Reyes, Yellowstone, Big Bend, and the Grand Canyon, although there are many parks I have not yet been too.

Here is a gorgeous picture of Arch Rock, a location my family and I hiked to at Point Reyes:

![Decorative: Arch Rock](arch-rock-point-reyes.png)

This picture does not do Yellowstone justice _at all_, but no one picture can:

![Decorative: Yellowstone](yellowstone-vista.png)
```

Page Media:
- _Arch Rock, Point Reyes National Seashore_ **as** _arch-rock-point-reyes.png_
- _Yellowstone Vista_ **as** _yellowstone-vista.png_

#### Options

Tags:
- landscape photo
- just for fun

#### Blog Item

Hero Classes: _none_

Hero Image: _none_

#### Frontmatter
```yaml
CLIP: title: Parks
media_order: 'arch-rock-point-reyes.png,yellowstone-vista.png'
taxonomy:
    tag:
        - 'landscape photo'
        - 'just for fun'
feed:
    limit: 10
```

### 10. Requesting Books

#### Content

Title: ```CLIP: Requesting Books```

Content: 
```md
CLIP: Have you ever found the perfect book or article, only to run into issues actually obtaining it from the library? Sooner Xpress and ILL may be able to help.

===

If you are looking for a resource the library owns, most likely your issue is either that, although it is supposed to be on the shelf, you cannot find it, or that it is currently checked out. You should first make certain that you are looking in the right place - check the Discover search results to see where the book is listed. If it isn't in the main library stacks it might be in a branch library, Special Collections, or Reserves. Special Collections books are non-circulating, but you can read them while you are at the library. Reserve books are placed there at the request of professors who will be requiring them for class. These books have a four hour checkout time, which means that, while you can't take it home with you for weeks on end, it will actually be available a lot more often.

Assuming the book is not in Special Collections or Reserves, you can request it via Sooner Xpress. The option to do this will be on the Discover page for the book. You can specify which library you want to pick it up from, and you will be notified by email when it is ready for you. This is great for reserving a popular book with a waiting list, for reserving a book when you don't come to the library very often, or for reserving a book you are having trouble finding.

If the resource you are looking for is not one we have access to, you can make an InterLibrary Loan (ILL) request. Even if you do not go to OU, many libraries participate in ILL, so check with your local library. You may realize you have access to a lot more books and articles than you thought you did! Before filling out an ILL request, make sure that you are not requesting a textbook or something we already have access to. For example, if we have a book on Reserve or in Special Collections, ILL will probably deny the request.

If you have any questions, please [contact us](https://libraries.ou.edu/content/contact-us). We are always happy to help you get access to the resources you want or need.
```

Page Media: _none_

#### Options

Tags:
- ou libraries

#### Blog Item

Hero Classes: _none_

Hero Image: _none_

#### Frontmatter
```yaml
CLIP: title: 'Requesting Books'
taxonomy:
    tag:
        - 'ou libraries'
feed:
    limit: 10
```
