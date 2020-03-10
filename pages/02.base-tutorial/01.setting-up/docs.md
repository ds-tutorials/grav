---
title: 'Setting Up'
media_order: 'check-for-updates.png,default-directory.png,fully-updated.png,grav-directory.png,install-grav.png,installation-settings.png,installatron-grav.png,no-directory.png,to-admin-panel.png,to-website.png,update-grav.png,update.png'
taxonomy:
    category:
        - docs
---

! Please note: This tutorial describes installing Grav using Reclaim Hosting, specifically through OU Create. If you are using this tutorial but wish to install Grav a different way, please refer to the [official documentation](https://learn.getgrav.org/16/basics/installation) for installation instructions.

## 1. Set up your domain

If you are currently affiliated with OU, you have access to a free subdomain of oucreate.com through OU Create/Reclaim Hosting (or an inexpensive domain of your own). If you have not yet claimed this domain, please set it up now following the instructions [here](https://create.ou.edu/docs/getting-started/signing-up/).

## 2. Install Grav

Once you have signed in to your dashboard on OU Create/Relcaim Hosting you will either see Grav listed under the Applications section or you can click on All Applications and find Grav from there.

![Button 'install this application' located at the top right corner of the Installatron Grav page.](./installatron-grav.png)

While most of the default settings for the installation are fine, there are a few we want to change.

By default, the installation will want to put Grav in a folder (directory) called _cms_.

![Input box for 'Directory (Optional)' contains the text 'cms.'](./default-directory.png)

You can choose instead to install Grav directly in your home folder by leaving the field blank.

![Input box for 'Directory (Optional)' contains no text.](./no-directory.png)

Or you can change the name of the folder. For this tutorial, we will name our folder _grav-demo_.

![Input box for 'Directory (Optional)' contains the text 'grav-demo.'](./grav-directory.png)

It is worth noting on the three screenshots above what the resulting URL is for each website. This is how you and visitors will access your site online.
- Default directory: ds-tutorials.oucreate.com/cms/
- Blank directory: ds-tutorials.oucreate.com/
- Grav demo directory: ds-tutorials.oucreate.com/grav-demo/

We also need to set the website name, as well as our full name, email address, username, and password, as shown here (but please use your own name and email address).

![Input boxes for Settings are filled out. Site Title is Grav Blog. Please fill out Full Name and Email Address with your own name and email. Username is admin. Password is hidden.](./installation-settings.png)

Finally, the only other setting we might consider changing here is the skeleton package. The default, GravCor + Admin, is not bad, but depending on what we want to do, a skeleton package might make setting up the website easier. For this tutorial we will stick with the default. 

!!!! You can learn more about skeletons in the mini-tutorial when it is released.

All we need to do now is press install.

![Button 'install' is located at the bottom left under the 'Advanced' installation options.](install-grav.png)

! Note that while the screenshots show the demo being installed at grav.ds-tutorials.oucreate.com, the actual demo is located at ds-tutorials.oucreate.com.

## 3. Check out the admin panel

Familiarity with the admin panel is important, as this is where we will spend most of our time building our website. You can access the panel directly by going to `your-website-url/admin`, or you can go to your grav application on the OU Create/Reclaim Hosting dashboard after installation. You will see links to access both your website and the admin panel. The first link will take you directly to your website.

![Link to website is the first of three links for Grav Blog. The format is domain.oucreate.com/installation-folder/.](to-website.png)

The second link will take you to the admin panel.

![Link to the admin panel is the second of three links for Grav Blog. The format is domain.oucreate.com/installation-folder/admin/](to-admin-panel.png)

When you click the link to the admin panel, you will be prompted to log in with the username and password you chose in the installation settings.

!!! The Grav documentation has a whole chapter dedicated to the [administration panel](https://learn.getgrav.org/16/admin-panel). It is worth skimming, at the very least.

## 4. Update Grav

Before we do anything else, we need to make sure that Grav is up-to-date. On your dashboard, click the _check for updates_ button.

![Button 'Check for Updates' is at the top right corner of the admin panel dashboard.](check-for-updates.png)

In this case, I have to do two updates. First, Grav itself has been updated to a new version. It is essential to always keep Grav updated to the latest version to minimize potential errors.

![Button 'Update Grav Now' is just below the 'Check for Updates' button.](update-grav.png)

When that update is complete, there are still normal updates required. Several of the packages (themes or plugins) that were automatically installed are not on the latest version. These updates are also important.

![Button 'Update' is at the bottom right of the Maintenance section.](update.png)

When that has finished, the dashboard will show that everything is up-to-date.

![The Maintenance section shows Grav is 100% updated.](fully-updated.png)

If you run into any issues using the admin panel, or just want to know more, you can check out the [documentation](https://learn.getgrav.org/16/admin-panel).