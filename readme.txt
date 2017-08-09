=== WP Twitter Users ===
Contributors: 0xTC
Tags: Twitter, Users, FollowFriday, profiles, badges, user, lists, showcase
Requires at least: 2.0.0
Tested up to: 2.8
Stable tag: trunk
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=6331357

Allows authors to showcase one or more Twitter accounts. Useful for creating Follow Friday lists in posts or pages.

== Description ==

Allows authors to showcase single Twitter users or create formatted lists of users shown in in badges using a simple shortcode.

You can choose from 10 profile templates or create your own custom template and put it in your theme's /wptu/ subfolder.

**Please read the installation manual and FAQ. You may find them insightful.**

== Installation ==

1. Upload/extract the `wp-twitter-users` folder to your `/wp-content/plugins/` directory.
3. **Make sure the `/xmlcache/` sub folder is writable! (Permissions set to 766 seems to work best)**
4. Activate the plugin through the 'Plugins' menu in WordPress.

**It is recommended to create an external cache path in order to preserve cached data between updates. Read the FAQ on how to enable this feature.**

== Frequently Asked Questions ==

= So, how do I use it? =

Just enter one or more twitter users in the shortcode `[ff xxx...]`. Example:

`[ff tcorp theemperfect]`

This will create two user boxes for the Twitter users "tcorp" and "theemperfect".

You can list as many users as you wish, but keep in mind that Twitter has a 150 requests/hour limit! If you create lists that have more than 150 users, the plugin will only list the first 150 users. You can always refresh the page an hour later and see if more users have been added to your post/page.

= Shortcode aliases and alternative input =

Instead of `[ff ...]` you can also use the following variations:

* `[#ff ...]`
* `[#followfriday ...]`
* `[followfriday ...]`
* `[twitterusers ...]`

All of the above shortcodes have the same result.

Usernames can be entered in a number of ways, all valid to the plugin. For example for the twitter user "tcorp" you can enter one of the follow variations:

* [#ff tcorp]
* [#ff @tcorp]
* [#ff http://twitter.com/tcorp]

= How do I preserve the cache between updates? =

If you wish to preserve your cached XML files due to Twitter limitations, create the following **writable** folder: **`/wp-content/cache/xmlcache/`**.

All the requested will now be cached in the **external cache path** if it is writable.

== Screenshots ==

1. Example of a template
2. more templates
3. How you enter values

== Changelog ==

= 1.0.0 =

* First build!

= 1.0.1 =

* Added Error capturing
* Prefered cache directory defined.
* Added option for external cache.

= 1.0.3 = 

* fixed typo

= 1.1.0 =

* Added support for tweetimag.es (3rd party twitter image provider)

= 1.1.1 =

* Added auto-cleanup feature for faulty requests that are already cached.
* Accommodates for "Twitter is Over Capacity" error.