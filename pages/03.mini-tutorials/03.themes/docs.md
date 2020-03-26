---
title: Themes
published: false
taxonomy:
    category:
        - docs
---

## What is a theme?

In Grav, themes determine what template options you have for pages and what the content in those pages will look like. The [Grav documentation](https://learn.getgrav.org/16/themes) on themes is very thorough. You might look at it for reference, but I would not feel any obligation to read through all of it. There is also a section more focused on using themes within the admin panel [here](https://learn.getgrav.org/16/admin-panel/themes).

## What is a Skeleton?

A theme skeleton generally involves a theme, sample pages, plugins, and pre-made configuration options. They often have a demo website so you can see what the skeleton looks like in practice. Even if you do not actually use a skeleton for a theme, you may find the sample pages or demo website useful in seeing what you can do.

Your primary options for using a skeleton are either downloading Grav with one already in place or manually adding one from a GitHub repository.

## Starting Grav With a Skeleton

Downloading Grav as a skeleton package is the most convenient option because everything will be set up for you. Even the default install from Reclaim Hosting is essentially a skeleton, albeit a very basic one. However, only a few of the skeletons out there are offered with an initial Grav install from Reclaim Hosting/OU Create. The corresponding demo sites for these skeletons are listed below.

* [Twenty](https://demo.getgrav.org/twenty-skeleton/)
* [Resume](https://demo.getgrav.org/resume-skeleton/)
* [One Page](https://demo.getgrav.org/onepage-skeleton/)
* [Photographer](https://demo.getgrav.org/photographer-skeleton/)
* [Learn2 with Git Sync](https://demo.hibbittsdesign.org/grav-learn2-git-sync/)
* [Open Course Hub](https://demo.hibbittsdesign.org/grav-open-matter-course-hub/)
* [Open MultiCourse Hub](https://demo.hibbittsdesign.org/grav-skeleton-open-matter-multi-course-hub-site/)
* [Open Publishing Space](http://demo.hibbittsdesign.org/grav-open-publishing-quark/)

When you are making a fresh install of Grav it is definitely worth checking out these websites first. If you know you want to use a theme/setup like on of them, choosing that package during install will make the initial setup for your website much easier.

## Adding a Skeleton After Installation

If you decide you want to use a skeleton after installing Grav or you want to use one of the other skeletons out there the setup is a little bit more involved but still reasonably simple.

1. Find the skeleton you want to use [here](https://getgrav.org/downloads/skeletons)
2. Download the zip file for the skeleton you want
3. Go to your File Manager in Reclaim Hosting/OU Create and navigate to your Grav install
4. Upload the zip file and extract it
5. Copy the _user_ folder from the skeleton folder into your Grav folder. Do not remove _user_ from the initial install folder before doing this. For example, if you are using a skeleton that does not automatically include the admin plugin, copying the plugin folder from the skeleton site to your installed site will add all of the plugins it has but it will not remove any plugins it doesn't. Therefore, you will still have the admin panel.
6. You can now delete the zip file and the extracted Grav folder

When using the sample pages in the skeleton as a reference for your own, make sure to switch to expert mode and check the frontmatter section in case there are options that are not shown in the user interface of the page editor. I have definitely had that be the case before.
