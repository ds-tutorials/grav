---
title: 'Basic Theme Customization'
published: false
taxonomy:
    category:
        - docs
---

Ideally your theme will have all the configuration options you want built into it.
It probably won't.

If it does: You can go to the _Themes_ tab, click on your selected theme, and make changes to the config options provided after the basic info. Remember to save your changes.

If it does not: Modifying a theme directly is risky business, because your modifications may well be overwritten whenever the theme updates. Some themes provide a _custom.css_ file that they leave blank so you can make changes that will not be overwritten. To find out, navigate through your file system to your grav install -> user -> themes -> quark (or other theme) -> css and look for a custom.css file. (Quark does have one of these). The file should be empty. If it has anything in it (that you did not add) that means that it is actually used for the theme (most likely) and that you cannot trust that it will not be overwritten in an update.

Granted, you should not trust that it won't be overwritten even if it is blank, because you never know, so after making changes save the file somewhere else so you will still have it just in case.

If there is not a custom.css file here are three options:
1. Don't customize.
2. Choose a different theme.
3. Go to Advanced Theme Customization

## CSS

You should probably at least know some very basic CSS and how it interacts with html. You do not have to feel comfortable writing whole webpages or even using most html or css options.

1. Get the basics of CSS from [W3Schools](https://www.w3schools.com/css/). You don't have to follow through the whole tutorial. Just read enough that you have an idea of what is going on and keep it for reference when you look up how to do specific things.
2. Get the basics of HTML from [W3Schools](https://www.w3schools.com/html). You definitely should not read the whole tutorial. I would focus on the first few sections: Basic, Elements, Attributes. Also make sure to check the sections about [Classes](https://www.w3schools.com/html/html_classes.asp) and [IDs](https://www.w3schools.com/html/html_id.asp). These tend to be referenced often in CSS.
3. Check out your webpage to see how everything interacts. Go to your webpage and either right-click and choose Inspect or, if that is not an option, look up how to inspect elements with your specific web browser. (Google is going to be your best friend.) The inspect column that opens up should be on Elements at the top and Styles at the bottom. You do not have to know what all of this means.

The important things:
- Ctrl/CMD + shift + C (or the little box and cursor icon): Click on this and then click on the part of the page that you want to modify. So, for example, if you think the navigation header color is boring, click on it. When you hover over things you will see that they are highlighted, so make sure that the thing being highlighted is what you want - so if you are interested in the whole navigation header, you want the whole thing to be highlighted if possible. If you hover over some of the text you will probably be shown an element within that navigation header, which is less helpful. Clicking will select the line where that element is introduced in the HTML (The top half, or Elements section)
- You can expand the HTML or go up a level until you find just the right element. Check out the styles to see what CSS is being applied to that element. This will also show you how it is being applied. For example, is the text this color because that color is set for the "p" element or because that color is set for a specific class, perhaps ".main-text". This will let you know what you want to overwrite in your custom CSS.
- Experiment! You can change the CSS within the Style section to see how something would look. Keep in mind that these changes will go away as soon as you refresh the page, so if you find anything you love, write it down somewhere else, too. The next stage of experimentation is adding the CSS you think you will need to the custom.css sheet, saving it, and refreshing your webpage.

Troubleshooting:
- Like any code writing, there will be issues. Things will break, changes won't actually change anything, and things will happen that you did not want. First, keep in mind that this is normal. Even the fancy programmers out there are constantly troubleshooting and looking things up.
- Set limits. Troubleshooting can be frustrating, especially when you don't fully understand what is happening with the HTML, CSS, or even potential underlying Javascript. I am speaking from experience here. I have customized themes to some extent, but there are some things I could not figure out. That is okay. If a particular change would be nice, give yourself a certain amount of time to experiment, look things up, and otherwise try to make it happen. If you still feel overwhelmed after this time is up, perhaps it is time to consider that thing as something that you won't be able to change.
- Another type of limit: Don't plan to change all the formatting etc. etc. For basic customization you want to focus on font color and background color primarily or perhaps exclusively. Don't try to get too fancy.
- Check to make sure that custom.css actually is being applied to the template
- Make sure that you saved
- Try doing a hard refresh
- Check to see if the change is listed in the Style section but has a strikethrough, indicating that something else is overwriting it
- Google things!
- Check the element type, the class, and/or the ID.

Ultimately, in most cases you will be able to change at least some things in your website. You may not change everything. You may not be completely satisfied. Keep in mind that the only way to be completely satisfied with how a website looks is to design it from scratch, and that is A LOT of hassle. Always settle for "good enough."

This may be less of a problem if you are used to editors that give you a limited set of options. For example, Grav provides a number of potential themes. Hopefully one is close enough to what you want, but none of them will probably be the absolute perfectest thing ever.

Particularly as a programmer (at least to some degree), I have a tendency to get very specific ideas of how I want things to look and act. Because I know it is possible to write the code that will generate that, I often feel stifled and dissatisfied when I am forced to settle instead of writing my code. However, as a programmer (at least to some degree), I am also well aware of just how much work it is to design something from the ground up, and even how difficult it is to build in varying degrees of customization. It can get really complicated! So find the theme that does what you want as much as possible and make some minor changes to the style if necessary. Be aware that the more you want to change things, the more complicated it will be, and the more code you will have to write.

If you must get really complicated, I will go over a few more things in Advanced Theme Customization, although I am not going to go into all of the details of basically creating your own theme.

If the theme you want does not have a custom.css file but you only want to make some minor changes, go on to Advanced Theme Customization anyway for a reference to theme inheritance.