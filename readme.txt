=== Banner Rotator FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, banner, maker, creator, rotator, slideshow, zoom, ken, burns, scroll, xml, portfolio, text, slide, page, button, background, transition, mask, effect, text, as2, preloader, photo
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

Maybe the most advanced Banner Rotator on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. The overall width and height can be customized up to 1680 x 1050 pixels. Choose from more than 100 transitions. Supports JPEG, BMP, GIF, PNG, SWF. Auto timing (as an option, each image will last according to the length of the text; if not, you will be able to specify the duration for each image, in seconds). Option to have random images and/or random transitions. Ken Burns and Zoom image effects. If the images are displayed in a random manner, the Banner uses a fair advertising policy (meaning you won't see an image twice until all other images are displayed). Any sizes can be used for the images - they will automatically be adjusted according to the imageFitting option. Every image can optionally have different particularities, different from the overall settings of the Banner, like image and text effects, transitions, text options. HTML/CSS formatted text.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/banner-rotator-fx.zip "Banner Rotator FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/banner-rotator.zip "Banner Rotator FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **banner-rotator-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Banner Rotator FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[banner-rotator-fx][/banner-rotator-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Banner Rotator FX part of your theme, edit the template files and add `<?php bannerrotatorfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Banner Rotator FX](http://www.flashxml.net/banner-rotator.html "Banner Rotator FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/banner-rotator-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/banner-rotator-fx/images/` and update the `wp-content/flashxml/banner-rotator-fx/images.xml` file accordingly

= Additional settings file =

To embed the Banner Rotator FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[banner-rotator-fx settings="settings2.xml"][/banner-rotator-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `bannerrotatorfx_echo_embed_code()` function call (for example `<?php bannerrotatorfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[banner-rotator-fx]` and `[/banner-rotator-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `bannerrotatorfx_echo_embed_code()` function call (for example `<?php bannerrotatorfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[banner-rotator-fx width="600" height="300"][/banner-rotator-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `bannerrotatorfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/banner-rotator.html "Banner Rotator FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/banner-rotator-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/banner-rotator.html "Banner Rotator FX") is the utility that helps easily customize your Banner Rotator FX to fit all your needs.