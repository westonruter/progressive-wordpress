=== Progressive WordPress (PWA) ===
Contributors: nico_martin, sayhellogmbh
Donate link: https://www.paypal.me/NicoMartin
Tags: PWA, Progressive Web App, Progressive Web Application, AMP, progressive, installable, add to homescreen, offline, offline usage, push notifications, OneSignal, manifest, web app manifest, serviceworker
Requires at least: 4.7
Tested up to: 5.0.3
Stable tag: 2.1.7
Requires PHP: 5.6
License: GPLv3
License URI: http://www.gnu.org/licenses/gpl-3.0.html

== Description ==

It has never been easier to add progressive web app features (PWA) to your WordPress website. It even supports [Accelerate Mobile Pages (AMP)](https://www.ampproject.org/) and is compatible with [OneSignal](https://onesignal.com/)!

= Add to homescreen =

Provide an **integrated** user experience!

Progressive WordPress makes it easy to encourage users to add your website to their homescreen. But that's not all. It also allows you to control the display behaviour of your website so it will be shown without any browser elements. Just like a native app.
= Offline usage =

Make your website **reliable**. Even on flaky internet connections!

No connection? No problem. Progressive WordPress pre-caches all critical assets of your website, as well as all visited resources. So if there's no internet connection it will serve the resources from the local storage. No more error downasaur!

= Push notifications =

**Send push notifications from the WP Admin interface!**

Keep your users **engaged** by sending push notifications!

You just published new content and you want to let everyone know? Why not send a push notification? Progressive WordPress has an integrated connection to Firebase that lets you manage registered devices and send push notifications to all or selected devices!

** Support for OneSignal**
Since Version 2.1.0 Progressive WordPress fully supports [OneSignal](https://onesignal.com/). It detects if the [OneSignal WordPress Plugin](https://wordpress.org/support/plugin/onesignal-free-web-push-notifications/) is active and uses their push messaging functionalities instead.

= ⚡ AMP ready =

Progressive WordPress is the first PWA-Plugin for WordPress that also supports Accelerated Mobile Pages!
It precaches required resources, it adds special AMP caching strategies and it registers the ServiceWorker and the Web App Manifest also on AMP Pages.
Progressive WordPress currently supports [AMP for WordPress](https://wordpress.org/plugins/amp/) and [AMP for WP – Accelerated Mobile Pages](https://wordpress.org/plugins/accelerated-mobile-pages/).

== Developers ==
Progressive WordPress offers a lot of possibilities for developers the extend it the way you need it.
[https://github.com/SayHelloGmbH/progressive-wordpress#developers](https://github.com/SayHelloGmbH/progressive-wordpress#developers)

== Screenshots ==

1. Discover what's possible
2. Make your website installable
3. Create a Web App Manifest..
4. ..no coding skills required
5. Manage the registered devices
6. create a push notification right from the admin intefrace
7. let the magic happen

== Installation ==

1. Upload the plugin folder to the `/wp-content/plugins/` directory or install it from the plugin directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Done

== Frequently Asked Questions ==

= Does this work on AMP sites? =

Yes! Progressive WordPress is the first PWA-Plugin that fully supports AMP! Register ServiceWorker on AMP, Precache AMP resources, use AMP as your web app start URL.
It's currently compatible with [AMP for WordPress](https://wordpress.org/plugins/amp/), [AMP for WP – Accelerated Mobile Pages](https://wordpress.org/plugins/accelerated-mobile-pages/) and can [easily be configured](https://github.com/SayHelloGmbH/progressive-wordpress#-amp-support) for any AMP plugin or theme.

= How can I use OneSignal? =

By default, progressive WordPress uses google Firebase to send push notifications. Since version 2.1.0 it also supports [OneSignal](https://onesignal.com)!

Progressive WordPress automatically detects if the official [OneSignal plugin](https://wordpress.org/support/plugin/onesignal-free-web-push-notifications/) is active and let's you use OneSignal instead of firebase.

= Nothing happens after installation =

1. Are you using a device/browser that supports serviceworkers? [https://caniuse.com/#feat=serviceworkers](https://caniuse.com/#feat=serviceworkers)

If they are both allright, please open an issue on [https://github.com/SayHelloGmbH/progressive-wordpress/issues](https://github.com/SayHelloGmbH/progressive-wordpress/issues)

== Contribute ==

A development version of this plugin is hosted on GitHub. If you have any ideas for improvements, feel free to dive into the code:
[https://github.com/SayHelloGmbH/progressive-wordpress](https://github.com/SayHelloGmbH/progressive-wordpress)

== Changelog ==

= 2.1.7 =
* removed jQuery! It's now only pure JavaScript
* conditional JS / CSS loading
* small stability improvements for the Site Icon
* httpsify start url

= 2.1.6 =
* AMP register ServiceWorker Bugfix

= 2.1.5 =
* Improvements for service worker registration
* Add to homescreen prompt fix

= 2.1.3 =
* New Filter to adjust the Site Icon: `pwp_manifest_icon`
* Fix for ServiceWorker registration inside subfolder
* Multisite fixes for OneSignal compatibility

= 2.1.2 =
* Multisite fixes for OneSignal compatibility

= 2.1.0 =
* AMP support ⚡
	* Detect if AMP is supported
	* Detect if current site is AMP
	* register ServiceWorker for AMP
	* register Manifest for AMP
	* Add caching strategies for AMP pages and assets
* Compatibility for [AMP for WordPress](https://wordpress.org/plugins/amp/)
* Compatibility for [AMP for WP – Accelerated Mobile Pages](https://wordpress.org/plugins/accelerated-mobile-pages/)
* Support for [OneSignal](https://wordpress.org/support/plugin/onesignal-free-web-push-notifications/)

= 2.0.1 =
* New caching strategy "Network Only"
* ServiceWorker minify
* Precache fixes

= 2.0.0 =
* Complete UI over-worked
* Settings renamed and rearranged
* Manifest Icon is now the same as Site Icon
* Added [Workbox v3.4.1](https://developers.google.com/web/tools/workbox/)
* Choose caching strategies for different request types
* Offline support for Google Analytics
* Future proof: Added support for the [PWA feature plugin](https://github.com/xwp/pwa-wp)

= 1.3.2 =
* Bugfix: Firebase Serverkey validation
* Bugfix: upload images on settings page

= 1.3.1 =
* messed up some SVN-deployment

= 1.3.0 =
* added default settings on activate
* Bugfix: Minifying JS threw an Uncaught SyntaxError

= 1.2.0 =
* added default settings on activate
* added UTM tracking for manifest starturl and push notification redirect url

= 1.1.2 =
* required php Version is now 5.6

= 1.1.1 =
* critical Bugfix: JavaScript error

= 1.1.0 =
* Bugfix: better way to check if files have to be regenerated
* Bugfix: PushPost not always registered
* Improvement: new manifest icon sizes

= 1.0.2 =
* Bugfix: CSS z-index for notification button

= 1.0.1 =
* Bugfix: Pushpost labels
* fixed spelling mistakes

= 1.0.0 =
* **Stable version 1.0.0**
* added multisite support
* Pushpost: send push notifications right from the post edit screen
* Added translation: de_DE
* Added translation: de_CH
* push button color input-type improvements
* add JS vars as `wp_add_inline_script`

= 0.7.0 =
* added a latest push log
* added a debug log
* using `WP_Filesystem` API instead of php `file_put_contents`
* Added "orientation" to manifest
* Added colorpicker to settings
* Fix: is_ssl() improvement

= 0.6.2 =
* Bugfix: featured image could not be changed if push notifications are enabled

= 0.6.1 =
* Bugfix: prohibit console error if sw not supported

= 0.6.0 =
* Added offline content
* select front page as offline Page
* Improvement: better hex check for manifest colors

= 0.5.1 =
* Bugfix: notification Button always visible

= 0.5.0 =
* Added push notifications!
    * let the user manage their subscription
    * manage all registered deivces
    * send push notifications to all or specific devices
* added ad status checks
* force the browser to unregister all other serviceworkers
* minor bugfixes and improvements

= 0.4.0 =
* you can now change the manifest start_url
* Bugfixes

= 0.3.0 =
* changed offline indicator
* added better instructions
* codepattern improvements

= 0.2.0 =
* added offline indicator
* Grammatical changes by [Mark Howells-Mead](https://profiles.wordpress.org/markhowellsmead/)
* "installable" is now optional
* Manifest Icon has to be png and min. 144x144px.

= 0.1.0 =
* Initial version