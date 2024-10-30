=== MP3 Player FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, mp3, player, free, flash, as3, xml, autoplay, audio, playlist, visualizer, play, auto, scroll, autoscroll, effects, shuffle, repeat
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

One of the most advanced MP3 Player on the web. Completely XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. It has autoplay, shuffle and repeat functionality with many customizable properties for the visualizer. The skin for the player and the playlist is customizable. The playlist has roll over/out effects and many different changeable properties. Other features are available on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/mp3-player-fx.zip "MP3 Player FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/mp3-player.zip "MP3 Player FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **mp3-player-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **MP3 Player FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[mp3-player-fx][/mp3-player-fx]` where you want the Flash to show up in your post/page
5. If you want to make the MP3 Player FX part of your theme, edit the template files and add `<?php mp3playerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your MP3 Player FX](http://www.flashxml.net/mp3-player.html "MP3 Player FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/mp3-player-fx/settings.xml`
7. To use your own music, upload it to `wp-content/flashxml/mp3-player-fx/assets/sounds/` and update the `wp-content/flashxml/mp3-player-fx/playlist.xml` file accordingly

= Additional settings file =

To embed the MP3 Player FX more than once, you will need another settings file. Let's assume your new file is called `settings2.xml`. Add `[mp3-player-fx settings="settings2.xml"][/mp3-player-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `mp3playerfx_echo_embed_code()` function call (for example `<?php mp3playerfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[mp3-player-fx]` and `[/mp3-player-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `mp3playerfx_echo_embed_code()` function call (for example `<?php mp3playerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[mp3-player-fx width="600" height="300"][/mp3-player-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `mp3playerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/mp3-player.html "MP3 Player FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/mp3-player-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/mp3-player.html "MP3 Player FX") is the utility that helps easily customize your MP3 Player FX to fit all your needs.