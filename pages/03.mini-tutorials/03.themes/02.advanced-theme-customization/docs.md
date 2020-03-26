---
title: 'Advanced Theme Customization'
published: false
taxonomy:
    category:
        - docs
---

- Grav has a [theme tutorial](https://learn.getgrav.org/16/themes/theme-tutorial) that guides you through creating a new theme using pure.css framework
  - Be aware that doing this would give you a clean slate, but you would then be much more on your own as far as CSS and templating
  - That is beyond the scope of this tutorial.
- We will build off of another theme. Pick the theme you like best but that you want to modify and use Grav's [theme tutorial](https://learn.getgrav.org/16/themes/theme-tutorial). The major difference here is that you will pick the inheritance option instead of the pure-blank option.
  - What will happen: When Grav looks for the appropriate template or CSS, it looks inside of the chosen theme folder. With inheritance, it will look first inside your theme, and, if it does not find the file it was looking for, it will continue to your original theme. This way you can make changes that will overwrite the original theme without having to directly change that theme. If the original theme updates you will receive the benefits of those updates (probably) without having your added content overwritten by the update as you would if you directly modified content in the original theme.
  - Keep in mind that you will have to use your file system for this and that you do have to use the console
  - Using the console in Reclaim Hosting/OU Create: Choose the Terminal option under the Advanced section. Type `ls` and press enter to see what files and folders are contained in the folder you are in. Look for your Grav install folder. Type `cd`, add a space, and then type the title of the Grav install folder. You can start typing this title and then press tab for auto-fill. Clicking enter will move you to that folder. 

To use some of the basic CSS mentioned in the Basic Theme Customization tutorial, you have a couple of options (assuming the theme does not already provide a custom.css file).
1. Create a new file in your theme folder/css called custom.css. Then add a line to the base twig template that adds that CSS to your pages.
2. Find the best CSS file to copy, copy that file into your own css folder and modify that as needed.

The first one means that you will be overwriting the base twig template. If an update makes changes here, you will not be getting those changes unless you manually reconcile them. Theoretically this could cause issues, especially since the base template is so important.

Potential work-around: have a second base template that extends the first and only adds the CSS. This might work.

The second option means that if an update makes changes to the chosen CSS file you will not get those changes. This is probably less concerning, but the level of concern may depend on the CSS file you picked.

- walk through both options

You can, of course, do much more complicated CSS than what is mentioned in the previous section. W3Schools is a very comprehensive guide, so knock yourself out if you enjoy playing with the CSS.

## Modifying Existing Templates

We will not go into how to create entirely new templates. That is a lot more complicated.

However, there may be some minor changes you would want to make to a template.

- Add a class or id to an html element so you can easily apply CSS to that section.
- Change hard-coded text
- Remove a section you find annoying or irrelevant.

You will want some familiarity with HTML and Twig. You do not have to be proficient in either to make basic changes, but do be aware of the limits in your knowledge. Knowing that you aren't sure what will happen when you change something means that you will exercise caution and restraint, testing carefully and not making huge changes. Thinking you know what will happen can lead to serious issues. (As a programmer sometimes, I find it helpful to remind myself that already written works are complicated and interconnected and that I have no idea what I am doing. While this does not stop me from trying to make changes anyway, it does encourage me to test things carefully, document changes I make, and expect the strange side effects that inevitably end up occuring.

## Adding Blueprint Options

You could get really fancy with this, adding things to the Twig template that connect to things you add in the blueprints. I'm not going into all that. 

The facts:

- The frontmatter defines a list of variables that are useful for that page. These variables are used by template(s) and/or plugin(s) that reference the page.
- The blueprint defines what configuration options you are provided in the frontmatter
- You do not have to have a blueprint to use the frontmatter!

For example, do I have any areas where I say switch to expert mode to make a change to the frontmatter? Find them!

In this kind of situation, the blueprint for the page does not specify that option, but you can still add it manually to the frontmatter. What the blueprint does is provide a user interface for various configuration options.

1. If there is not a blueprint for the template, you can create one.
2. If there is already a blueprint, copy it and then add to it.

- walk through examples

This was only a brief introduction to what you can do with templates and blueprints. It should be enough to allow you to make the most pressing minor changes you might want for a theme. You can, however, get really fancy if you want. At that point you are moving far beyond this tutorial and deeper into the realm of web designing. There are many sections in the Grav tutorial that may be relevant and many issues you will likely run into. Whether or not you get fancy, remember the importance of doing a Google search or three to see if someone else encountered the same problem you did.

If you can't find anything, you can specifically check forums for Grav, or StackOverflow, and if they have nothing you can post your own question. (Keep in mind for StackOverflow especially, you want to be very sure that no one has asked the question before. Be thorough in your searching, because they will rip you a new one if you a repeat a question. If your question is new, they will tend to be as helpful as possible, but they get mad when they feel like you are wasting their time by not doing your own research before asking). You can also ask me if you run into any issues (and, especially if the issue is related to something here not being suitably clear, please do!).