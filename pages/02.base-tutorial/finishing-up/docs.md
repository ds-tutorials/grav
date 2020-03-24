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

### Folders

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

For each of the following pages, go to the _Advanced_ tab, change the _Parent_ (under _Settings_) to _/library_, and save.
- Library Resources and Research Help
- Library Workshops
- Requesting Books
- Telescopes

- change only one, navigate to see what happened, then change it back

We can keep creating folders and moving pages to create whatever file structure we like. When making new pages, we can specify any of these folders as the parent.

### Numeric Prefixes

Within each folder, Grav sorts the pages alphabetically. You may notice that the _Library_ folder is an exception to this. Click on the folder and go to the _Advanced_ tab. Under _Ordering_ you can see that _Folder Numeric Prefix_ is enabled and that the folder is listed as _01.Library_ under _Sortable Pages_ while all of the other pages are listed under _Unsortable Pages_. What this means is that if we navigate to the `user/pages` folder outside of the admin panel we will find that the folder is named `01.library`. If a folder name starts with numbers and a period, Grav knows that this is solely for ordering purposes and will remove the characters when displaying the actual name.

The key point here is that we can enable folder numeric prefixes for all of our pages and define whatever order we want. When creating a blog there is an even more convenient option, but we will go over how to sort with the numeric prefixes first. It is also worth noting that the other option only exists within the admin panel, whereas numeric prefixes will sort the folders themselves, whether we are using the admin panel or an ordinary file explorer to view them.

We can try numeric prefixes starting with our first post, _Grav_. Going to the _Advanced_ tab we see the same sorting options as we did for _Library_, except that the _Grav_ page does not have the numeric prefix enabled. Start by enabling it and saving the page. Grav is now listed as `02.Grav`, just below `01.Library`. Since _Grav_ is our first page we probably want it at the bottom of the list. Our most recent pages are the most likely ones to need editing, so it makes sense to have them at the top. However, we can easily change the order by dragging and dropping the pages under _Sortable Pages_.

Since we do have a more convenient option, we disable _Folder Numeric Prefixes_ before saving and going back to the _Pages_ tab. This time we want to take a look at the _Blog_ folder.

When creating a blog, however, there is an even more convenient option we can choose. Presumably we would want our pages to display in the order that they were posted. Then we could easily find the most recent post by looking at the top of our folder. This would actually be rather complicated to do manually, as we would have to start our first post with the highest number, even though we would not know what the highest number would actually be. What we could do is sort the pages satisfactorily for now using the numeric prefixes, and then drag and drop each new folder within the sorting section.

Fortunately, the admin panel provides the option to sort folders based on 

-	Numeric prefixes: Remember to set the override visible to disabled when enabling numeric prefix. Otherwise the page will be added to a Blog dropdown in the navigation header.
