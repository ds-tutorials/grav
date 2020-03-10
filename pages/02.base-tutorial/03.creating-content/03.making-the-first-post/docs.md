---
title: 'Making the First Post'
media_order: 'add-post.png,added-tags.png,adding-media-and-credit.png,after-summary-delimiter.png,blog-first-post.png,first-post-image.png,first-post.png,first-tag.png,grav-content.png,navigation-dropdown.png,setting-hero-image.png,summary-delimiter.png'
taxonomy:
    category:
        - docs
---

No blog would be complete without posts. The template for a blog post is the _Item_ template. We can create a new page for our post the same way we added a blog page.

![The Add Page dialog box. Page Title: Grav. Folder Name: grav. Parent Page: --> (blog) Blog. Page Template: Item. Visible: No.](add-post.png)

I decided to name the first post _Grav_ since we are talking about how to use Grav. As before, the folder name is automatically generated, but this time we need to change the parent page from `NOCLIP \ (root)` to `NOCLIP (blog) Blog`. If we added the page to the root of our website it would show up as another page like _Home_ and _Typography_. Adding it to _Blog_ makes it a sub-page of that page, and because the _Blog_ template references a collection of its children (sub-pages), our new page will be displayed on our blog.

We also need to change the page template from _Blog_ to _Item_ and to set the page not to be visible. Visibility determines whether or not the page is displayed in the navigation. If we set the post to be visible, then mousing over the word _Blog_ in our navigation bar will display a dropdown menu we can use to access the page.