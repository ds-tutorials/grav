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
- _Total Solar Eclipse 2017, Wyoming_ as _eclipse-2017.png_

#### Options

Tags:
- tutorial
- markdown
- astronomy

#### Blog Item

Hero Classes: none

Hero Image: none

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
- _Yellowstone_ as _yellowstone.png_

#### Options

Tags:
- the carpentries
- landscape photo
- yellowstone

#### Blog Item

Hero Classes: `CLIP: title-h1h2 text-light overlay-dark-gradient`

Hero Image: yellowstone.png

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

### x. title

#### Content

Title:

Content:

Page Media:

#### Options

Tags:

#### Blog Item

Hero Classes:

Hero Image:

#### Frontmatter

### x. title

#### Content

Title:

Content:

Page Media:

#### Options

Tags:

#### Blog Item

Hero Classes:

Hero Image:

#### Frontmatter

### x. title

#### Content

Title:

Content:

Page Media:

#### Options

Tags:

#### Blog Item

Hero Classes:

Hero Image:

#### Frontmatter

### x. title

#### Content

Title:

Content:

Page Media:

#### Options

Tags:

#### Blog Item

Hero Classes:

Hero Image:

#### Frontmatter

### x. title

#### Content

Title:

Content:

Page Media:

#### Options

Tags:

#### Blog Item

Hero Classes:

Hero Image:

#### Frontmatter












### x. title

#### Content

Title:

Content:

Page Media:

#### Options

Tags:

#### Blog Item

Hero Classes:

Hero Image:

#### Frontmatter