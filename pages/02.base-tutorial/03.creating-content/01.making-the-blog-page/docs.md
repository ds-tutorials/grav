---
title: 'Making the Blog Page'
media_order: 'add-page-settings.png,add-page.png,blog-config.png,blog-page-content.png,expert-mode.png,header-demo.png,page-editor.png,result-blog.png'
taxonomy:
    category:
        - docs
---

Our first step is to add the blog page. This is where all of our future posts will be listed. To add a blog page, first click the _Add_ button on the _Pages_ tab.

![Button 'Add' is at the top right on the Pages tab.](add-page.png)

We have to choose a title for our page. I chose _Blog_ and the folder name automatically constructed itself as _blog_. We also have to set the template to use as the _Blog_ template. The other settings are good the way they are.

![Page settings are: Page Title: Blog; Folder Name: blog; Parent Page: / (root); Page Template: Blog; Visible: Auto.](add-page-settings.png)

## The Page Editor

After clicking the _Save_ button at the top right, the page editor will look like this.

![Various sections on the page editor are highlighted. Save button (5) is at the top right. Below that are tabs (3) with Content, Options, Advanced, and Blog Config. To the right of that is the editor mode toggle (4). Below that is the Title (1), with the input text currently 'Blog.' Below that is the markdown editor (2). At the bottom is the page media (6) section.](page-editor.png)

1. **Title**. This is automatically filled with the title we chose. We can change it at any time if we want a different title.
2. **Markdown Editor**. This is where the content of the page goes. Grav uses markdown to format text. The Grav documentation includes a very handy [markdown reference](https://learn.getgrav.org/16/content/markdown). There are also markdown editors you can use instead if you prefer. I found that once I got used to markdown I had no problems with the built-in Grav editor, but a lot of this will come down to personal preference.
3. **Tabs**. All pages will have _Content_, _Options_, and _Advanced_ tabs. _Options_ and _Advanced_ make it easy to change various settings for the page, although the defaults are often perfectly fine. Some pages will also have a special tab. For the _Blog_ page it is the _Blog Config_ tab. We will take a closer look at this in a moment.
4. **Editor Mode**. By default, the content editor is in normal mode. Putting it in expert mode will reduce the number of tabs and configurable options, but will allow us to directly edit the "frontmatter" of the page. Essentially, the frontmatter is a list of settings written in a special format at the top of the page. Using the normal editor mode obscures this by providing a user interface for setting these options. Occasionally, however, we may want to switch to expert mode in order to set an option that is not available in the user interface.
5. **Save Button**. This is the most important button on the page! Remember to save early and save often. You will also have noticed this button on the plugin and theme configuration pages. Any time we make a change, we need to save it by clicking this button.
6. **Page Media**. This is where you can add media that you want to embed in your page.

## Adding Some Content

The blog page is not supposed to take a lot of content. A heading and subheading is all it really needs. In markdown, headings are denoted with the hashtag symbol. Type

```md
CLIP: # My Example Blog

## Learning to use Grav
```

![The above text - '# My Example Blog \n\n ## Learning to use Grav' - is shown typed into the markdown editor.](blog-page-content.png)

This will render as

![Visual representation of the markdown.](header-demo.png)

## Testing Expert Mode

After saving, we can take a look at the _Blog Config_ tab.

![The Blog Config tab is shown. There are three sections - Hero Section, Configuration, and Content Definition.](blog-config.png)

There are a lot of options here. Fortunately, the default settings are usually good to start out with, so all you need to do is glance over this tab for now. Some of the settings define the collection of blog posts. Some others provide settings for enabled plugins.

If we switch to expert mode, we can see how these settings are provided in the frontmatter. Although we will not have to edit them while in expert mode, this will help demystify the frontmatter, which may help in the future if we come across something we cannot modify from the provided user interface.

![With Expert Mode toggle is selected (on the right in-line with the tab headings). The Content tab is selected, and the Frontmatter section is shown, which replaces the Title section shown in Normal Mode.](expert-mode.png)

Now we only have _Content_ and _Options_ tabs. On the _Content_ tab, the _Title_ section has been replaced with a _Frontmatter_ section, which defines the title and some of the options we saw on the _Blog Config_ tab. You may notice (especially if you took a look at the Options and Advanced tabs) that not all of the settings are listed here. If a setting is not explicitly defined in the frontmatter, Grav will automatically use the default.

Since the normal editing mode will be much more useful to us in general, we can go ahead and switch back. If we navigate to our website, it should look like this:

[ui-browser address="http://grav.ds-tutorials.oucreate.com/grav-demo/blog"]
![The Website Blog page (not the Home page) is shown. The content (title and subtitle) we added is featured prominently.](result-blog.png)
[/ui-browser]