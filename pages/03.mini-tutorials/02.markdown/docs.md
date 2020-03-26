---
title: Markdown
published: false
taxonomy:
    category:
        - docs
---

## Basics

- If you are unfamiliar with markdown, read [this page](https://learn.getgrav.org/16/content/markdown)!
- If you are familiar with markdown, keep it as a reference.

### Markdown Extra

- you can enable markdown extra if you want to
- [this page](https://michelf.ca/projects/php-markdown/extra/) (also linked to from the Grav markdown documentation) has more info about it. Honestly you probably won't need it, but if you do you can enable it
- On the admin panel, go to the _Configuration_ tab and choose _System_, then find the _Markdown_ section.

### Best Practices

- because the idea behind markdown is to create web rendered content that can also read easily as plain text, many of the fancy things you can do with markdown (like the shortcodes we will discuss or markdown extra) may detract from that. It is up to you what your priority is
- Extending the above, different websites have different "flavors" of markdown. For example, some of the things you can do by default with Grav markdown is not an option with GitHub flavored markdown. But is compatibility worth losing the additional functionality? How likely is it that you will be migrating this content elsewhere?

It's really up to you what you do, but I would strongly recommend learning the very basics of markdown and leaving it at that, only looking for something extra when you feel like you really need it. At the very least this will lessen the learning curve, as you will have less you feel you have to learn all at once.

### How do I remember all this?

The good new is, you don't have to. For all the basic types of things you would want to include (which should be sufficient for most pages), the bar at the top of the content editor has options. Clicking these will provide the markdown syntax necessary.

### Escaped Character

You may notice that certain characters, like the asterisk \*, are used in markdown syntax. So what happens when you actually want to include an asterisk in your text? That is where the backslash comes in handy. For example, the above asterisk was written as `\*`.

## Embedded Content

In general you can embed other webpages using html. [W3Schools](https://www.w3schools.com/html/html_iframe.asp) is your best guide.

The markdown editor in Grav includes a button for embedding a YouTube video if you have the YouTube plugin installed. Another plugin called Embed is available, which provides markdown code for embedding content. This one does not add a button to the editor, but it uses the same code format as the YouTube and it documents its use in its README. These are good options if you are trying to avoid HTML.

## All That Fancy Stuff

Shortcodes are (literally) short codes you can add to your markdown to make it do fancy stuff.

### Shortcode Core

- adds features like underlining, changing font size, text alignment, and more
- check out the [README](https://github.com/getgrav/grav-plugin-shortcode-core/blob/master/README.md)

### Shortcode UI

- fancy user interface options: tabs, accordion, browser wrapper, and more
- check out the [README](https://github.com/getgrav/grav-plugin-shortcode-ui/blob/master/README.md)

### Some Other Fancy Markdown Plugins

- [Markdown Collapsible](https://github.com/X-Ryl669/grav-plugin-markdown-collapsible/blob/master/README.md) - lets you create collapsible blocks of text
- [Markdown Color](https://github.com/getgrav/grav-plugin-markdown-color/blob/master/README.md) - lets you change the color of your text
- [Markdown Details](https://github.com/bitstarr/grav-plugin-markdown-details/blob/master/README.md) - based on Markdown Collapsible, different type of collapsible text blocks
- [Markdown Spoilers](https://github.com/regaez/grav-plugin-markdown-spoilers/blob/master/README.md) - lets you hide spoiler content
- [Markdown Task Lists](https://github.com/funkjedi/grav-plugin-markdown-tasklists/blob/master/README.md) - lets you make task lists with checkboxes
- [Shortcode Owl Carousel](https://github.com/getgrav/grav-plugin-shortcode-owl-carousel/blob/master/README.md) - lets you make a carousel of images