# WP Reading List


WP Reading List is a WordPress plugin designed to help organize and display books, magazines, articles, and anything else that you have read lately.  This plugin allows users to display what they have read, attach text like a review or notes to it, and provide a link to where visitors can find the piece.  The plugin comes bundled with three existing templates, complete with easily customizable CSS.

The concept for this project stemmed from Andrew Spittle's repository on github, https://github.com/andrewspittle/reading-list

## Installation

1. Install the plugin by searching for "WP Reading List" in the WordPress.org plugin directory  **or**  upload the `wp-reading-list` plugin folder, available here: `http://wordpress.org/plugins/wp-reading-list/`, to the `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Set the plugin settings via the submenu "WP Reading List" under "Settings" in the WordPress admin menu
4. Add Reading List items in the "Works" tab
5. View your Reading List items at "mydomain.com/reading-list/"

# Frequently Asked Questions

## How do I see my WP Reading List items?

After activating the plugin, publish a reading list item or two under the "Works" tab in the WordPress admin menu and then navigate to "mydomain.com/reading-list/" (or to "mydomain.com/?post_type=works" if you are using the "default" permalink structure.  Adding the "/reading-list/" or "/?post_type=works"to your site's base url directs users to your reading list items.  You can then add this url to your custom menu to make it easier for users to get to.

## Why doesn't "mydomain.com/reading-list/" or "mydomain.com/?post_type=works" work? **A.K.A.** Why is my website returning a 404 "Not Found" error when I try to view my reading list? 

If this is the case, simply go to "Settings" and then "Permalinks" and hit save (you do not have to change any settings).  This refreshes your website's rewrite rules and now "mydomain.com/reading-list/" or "mydomain.com/?post_type=works" should work.  Otherwise, make sure you have at least one published reading list item.

## If I deactivate/delete the WP Reading List plugin will I lose all the reading list items and authors I have already created?

If you deactivate or delete the plugin, you will not lose the content you have created but you will lose your plugin settings.

## Why aren't my widgets or sidebars displaying on the WP Reading List layout view?

At this point, the plugin does not support widgets or sidebars in its templates due to difficulty organizing the lists due to the unpredictability of widget/sidebar sizes.

## What can I do if I want to change the look of the Reading List layout to better fit with my theme? 

There are several options available in the WP Reading List admin settings to help the reading list layouts fit smoothly into any existing theme.  In addition, the templates have been highly detailed in terms of extra id's and classes for easy customization via CSS.  Many themes have a "Custom CSS" tab built into the admin menu where you can add your changes.  Otherwise, you can always place your modifications within the "style.css" file of your parent or child theme.

## How can I change the default WP Reading List image?

There are two options: 1) You can use the settings in the admin panel and use the file uploader there. 2) You can use a file manager and go to "wp-content/plugins/wp-reading-list/wprl-theme/" and replace the "default.png" image with your image of the same name.  It is recommended that you choose a default image with a 3:4 aspect ratio (width:height) to match the other cover images.

## The "Works", "Authors", "Types", and "Reading List" terminology is confusing.  Is there a easier way to think of these things?

Yes. Think of "works" as specialized "posts" and similarly of "authors" & "types" as different kinds of "tags".  The "Reading List" and "Reading List Items" is a phrase which tries to include all kinds of reading materials such as books, magazines, articles, etc.

## How do I use the WP Reading List shortcodes? 

The WP Reading List shortcode embeds a list of items on a page or sidebar widget according to both the plugin settings in the admin panel and the parameters passed to the shortcode.  The format is: [wprl layout="plain" number="10"].  At this time, the only format available is "plain" but you can specify any number for the number of works displayed. (*Note, -1 returns all works.)



# Changelog

## 3.0 
* Added image uploader for default cover image
* Added shortcode support for embedding plain reading list
* Fixed whitespace issue in source code
* Fixed issue with grid view layout

## 2.2.3 
* Fixed information fields not displaying in works archive

## 2.2.2
* Added more meta fields showing in single works template

## 2.2.1 
* Added css id for use in styling plugin templates

## 2.2 
* Fixed bug in grid view for paginated views
* Fixed bugs resulting from adding language support
* Added way to update database without removing previous settings in admin panel

## 2.1.1 
* Added further language support

## 2.1 
* Fixed bug which did not show the last row of details in the grid view
* Added multi-language support

## 2.0.1 
* Fixed minor redirect bug

## 2.0 
* Fixed bug which removed commenting from a site when installed
* Fixed permalink issue so the plugin now displays regardless of permalink setting
* Added "work types" so that a user can add classifications like "journal", "magazine", "book", etc.

## 1.3
* Fixed minor bugs from 1.2
* Improved terminology and taxonomy.  Deleted all references to "books" in favor of "works"
* Added to Readme

## 1.2 
* Added native update feature for future versions of the plugin
* Added admin feature for links to author archives
* Fixed small bugs since 1.1
* Sharpened default image and screenshots
* Added support for page ranges
* Improved user input sanitation and validation

## 1.1 
* Added code documentation and improved the WordPress Readme file
* Fixed an activation problem
* Removed delete items with uninstallation of plugin function
* Added a header picture and screenshots
* Added missing validate function for admin setting
* Finished "author" view template
* Fixed several display-related bugs
* Minor edits

## 1.0 
* First Stable release

# Upgrade Notice 

## 3.0 
Added shortcodes and updated default cover image options

## 2.1 
Fixed bug with grid view

## 2.0.1 
Fixed minor redirect bug in 2.0

## 2.0 
Fixed permalink issue and commenting bug

## 1.3 
Fixed bugs from 1.2 and improved taxonomy and terminology

## 1.2 
Added built-in update feature for future versions of the plugin and fixed small bugs

## 1.1 
Fixed activation problem and fine-tuned plugin code from version 1.0
