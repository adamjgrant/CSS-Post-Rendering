Demo
====
http://ajkochanowicz.github.com/CSS-Post-Rendering/

About
=====
This is a demonstration of a CSS trick to optimize page speed.

I noticed that my sites' main css files continuously grow larger as I need to
style more and more elements. However, often these styles are applied to just
a few elements rarely appearing in the site or further down the page.
By splitting these styles into additional CSS files further down the DOM, the
page loads first, only with the styles it really needs.

Graceful lazy-loading
=====================
To combat the problem of elements "jerking" into place once their styles have
loaded, one can use special rules to hide and style content, later resetting
these rules in secondary stylesheets.
