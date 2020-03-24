---
title: 'Finishing Up'
taxonomy:
    category:
        - notes
---

Now that we have a set of sample posts to work with there are only a few more things to do before we have a properly functional blog.

## Organization

By default Grav sorts all the blog posts alphabetically in the blog folder. With only eleven posts this isn't too bad, but it could become very annoying to navigate as we create more and more posts.

! To view a list of all your pages, go to the _Pages_ tab in the admin panel and click on the _plus_ icon next to _Blog_. This is your current folder structure.

There are two main options to make these files easier manage: Create folders inside the blog folder for additional structure and/or enable numeric prefixes to specify your own order of pages within a given folder.

### Using Folders

There are a few things to note before we start adding folders. First, the folder name will show up in the URL for the given page, so you probably do not want to name the folder anything really weird. Second, the way our blog looks for posts involves searching only the _Blog_ folder itself. We will need to change this to a recursive search: That is, the blog will look for any posts in the _Blog_ folder, then any posts within any folders in the _Blog_ folder, and so on.

#### Setting up recursive search

1. In the admin panel, go to the _Blog_ page.
2. Click on the _Blog Config_ tab.
3. Under _Content Definition_ the first option is called _Items_. Currently it should say `- '@self.children'`. Change this to `- '@self.descendants'`. Metaphorically, descendants tells Grav to look not just for children but for grandchildren, great grandchildren, and so on within the folder.
4. Click **Save**

#### Adding folders

Our blog posts currently fall into three broad categories: Posts about OU Libraries, tutorial/information posts, and a couple of random "fun" posts. We will add a folder for our posts about OU Libraries.

1. On the _Pages_ tab, click on the downward arrow on the right of the **Add** button and choose _Add Folder_.
2. Name the folder _library_ and choose _/blog_ as its parent page.
3. Go to the _Options_ tab for the new folder and click choose _No_ for _Published_. This ensures that the folder will not be displayed as another post on our blog page.
5. Save the folder



-	Blog structure: Make the blog use descendants instead of children (recursive). Add or move a page to the unpublished folder. It will display the folder name (or chosen slug) in the URL
-	Numeric prefixes: Remember to set the override visible to disabled when enabling numeric prefix. Otherwise the page will be added to a Blog dropdown in the navigation header.
