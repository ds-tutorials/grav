---
title: 'Grav Tutorial'
taxonomy:
    category:
        - docs
menu: Introduction
child_type: docs
subtitle: 'Build your own website with Grav'
intro: '1'
level: beginner
updated: '2020-03-09'
created: 'Theo Acker'
---

## What is Grav?

To quote the Grav documentation:

> Grav is a **Fast**, **Simple**, and **Flexible** file-based Web-platform.

If you have heard of Wordpress, Grav is very similar. It streamlines website building, allowing users to create their own without requiring previous coding knowledge or experience.

## What to Expect

This is not a reference guide to Grav. Grav has **very** thorough [documentation](https://learn.getgrav.org/16) which I strongly recommend using as a reference whenever you run into questions or problems. It is also worth looking over the documentation in general, but do not feel compelled to read all of it, and you certainly should not feel bad if you do not understand all of it. Some of the Grav documentation has very high-level information you will likely never need, and some of it may have information that will make sense once you have some more experience with Grav. As long as you are able to get Grav up and running, you will pick up knowledge and experience as you go. As with any complicated software, trying to learn everything all at once would be counter-productive. As a computer programmer, trust me, these things take time - lots of time.

Fortunately, you do not have to be a computer programmer or know any programming languages to make effective use of Grav. This leads me to the purpose of this tutorial. Rather than a reference guide, it is an instruction manual to get you started with the basics you need to put together a simple website. If that is all you need, great! If not, you will be in a better position to use other reference materials to expand your knowledge and the capabilities of your website. Keep in mind, the fancier you want your website to be, the more work you will have to put into it.

### Base Tutorial

The base tutorial is the first one you will want to work through. This will walk you through setting up Grav and building a simple blog-style website.

### Mini Tutorials

!!! The mini tutorials are currently under development.

These tutorials will extend the base tutorial, using the framework we will have already buit. There is no need to do all of them - just pick whichever ones look like they might come in useful.

I will include links to various references throughout the tutorial as they come up and as the mini tutorials become available.

If you are interested in contributing to the mini tutorials, please contact digitalscholarship@ou.edu.

## Additional Resources

These are listed in order from most important/least complicated to least important/most complicated.

- **[Grav.](https://learn.getgrav.org/16)** Naturally this is the most important documentation.
- **[Markdown.](https://learn.getgrav.org/16/content/markdown)** Grav content is written using Markdown. If you have seen HTML, Markdown is a lot simpler, while still providing a lot of versatility. The Grav documentation includes a helpful page on Markdown syntax.
- **[YAML](https://learn.getgrav.org/16/advanced/yaml)** is how Grav defines various configuration settings for the system, website, themes, plugins, and individual plugins. Much of this is hidden with the user interface of the admin panel, but occasionally it may be useful to interact directly with the YAML. The Link above will take you to the Grav documentation page for YAML syntax. Arguably [this page](https://learn.getgrav.org/16/basics/grav-configuration) about Grav configuration will be more helpful/give you a better idea of how YAML is used.
- **[HTML](https://www.w3schools.com/html/default.asp)** (Hyper Text Markup Language) defines the structure of webpages. Grav will accept HTML in place of Markdown, although you probably will not have much need to use it directly in page content. HTML can be particularly useful for understanding Grav templates and for modifying theme styles. It is entirely possible to avoid HTML entirely while using Grav, however. The link above will take you to W3Schools, an excellent source of reference and tutorial materials for web languages.
- **[CSS](https://www.w3schools.com/css/default.asp)** (Cascading Style Sheets) describes how HTML elements are displayed on screen. This includes colors, fonts, and much more. With a _very_ basic knowledge of HTML and CSS, you can add some simple customization to your website. W3Schools is an excellent resource for learning or looking up information about CSS.
- **[Twig](https://twig.symfony.com/doc/2.x/)** is a templating engine for PHP, which is a programming language. Grav templates are written using HTML and Twig, so if you decide to do any templating, you can rely on the much simpler Twig syntax instead of learning PHP.
- **[JavaScript](https://www.w3schools.com/js/default.asp)** is the programming language of HTML and the web. Grav templates can make use of JavaScript to add dynamic and interactive behavior to your website. It is not necessary to learn this in order to work with Grav, but if you want to, W3Schools is the best place to start.
- **[PHP](https://www.w3schools.com/php/default.asp)** Like JavaScript, PHP is a programming language (specifically a "server scripting language") that can add dynamic and interactive behavior to your website and can be learned through W3Schools. Since Grav uses Twig to provide PHP capabilities in a simpler format, this is the least likely to be useful to you.

