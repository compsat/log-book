# Log Book

Repository for CompSAt's Log Book

## Setting up the repository on your Wordpress folder

We will be using the local Wordpress environment for developing the website. In Wordpress development, the files that we'll be editing will mostly be in the wp-content folder, namely the plugins (if we have custom plugins) and themes (which we will most likely make).
Hence, this repository is **actually just the wp-content folder**, so please follow the steps below for setting up:

1. To set up Wordpress with XAMPP, follow the instructions in **parts I and II only**
[in this document](https://docs.google.com/document/d/1PPHta-pA0GhtGR3U4RmY1adnWcsBpV11fung7SqZpBA/edit#). 
Note that this doc can also apply if you will be using MAMP.
2. In your Wordpress directory, rename the `wp-content` folder to `wp-content-old` or whatever name you want it to be.
3. Still in the directory, clone this repository by running `git clone https://github.com/compsat/log-book.git`.
4. Rename the folder of the cloned repository (e.g. `log-book`) to `wp-content`. **This step is important for your Wordpress to still work, as it really looks for a folder named `wp-content`**.
5. If initially going to your Wordpress website on your browser will not work, don't worry. Just go to your admin page, and check the plugins and themes there. I think just refreshing the themes and plugins pages in the admin will make it work, as long as you won't see errors like "The active theme is broken. Reverting to the default theme" anymore in the admin.

Please note that your database won't be synced with the databases of the other developers, so you'll essentially be making your own posts.

## Installing Plugins

If you find a plugin that you think will be helpful for this website, you can find instructions on how to install it 
[here](https://wordpress.org/support/article/managing-plugins/) or manually installing it
[here](https://www.dummies.com/web-design-development/wordpress/templates-themes-plugins/how-to-install-wordpress-plugins-manually/). 
However, we want to make sure that the other developers will have it installed.

1. Install the plugin by following the instructions in the links above.
2. The installed plugin should be seen in the wp-content/plugins folder. Running `git status` should show the new plugin.
3. Run `git add [name_of_new_folder]` to add the new plugin to the commit stage.
4. Run `git commit -m [commit_message]` to make the commit.
5. Push the changes to the remote repo by running `git push origin [branch_name]`.

## Making changes to your custom theme

This should be straightforward and the same as the instructions above. Changes you did to the PHP/HTML/CSS/JS files in the theme
folder should be reflected in the `git status`.
