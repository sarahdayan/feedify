# Feedify
Feedify is a JQuery plugin inspired by Instagram's "stick to top then drop" effect.
While scrolling your feed, the header remains stuck to top, then is pushed away by the new item.

It comes with a beautiful yet optional theme which is everything you need to build a good-looking, functional feed of whatever you want.

## Features

### Fully responsive

The web is responsive now, there's no turning back.
Feedify goes with the flow.

### Cross-browser

Feedify works on all the most recent browsers,
and degrades gracefully down to IE9.

### Feedify theme

You don't need to be a front-end genius to make pretty things. Feedify comes with an optional theme.

### Flexible

Whatever your coding style is, Feedify respects it. Just add the right classes on your markup to make it work.

## How to use Feedify

### Include JQuery and Feedify

Feedify works with JQuery, so you'll need to add JQuery then Feedify for it to work properly. Be careful if you use multiple JavaScript libraries: Feedify is made to avoid conflicts, but you never know what might happen.

<pre><script src="http://code.jquery.com/jquery-latest.min.js"></script>
<script src="js/feedify.min.js"></script></pre>

### Build your feed

As developers, we like to remain totally free with our code. Some of us will rather keep things awfully simple, while others need extra markup. Some are totally sold with HTML5, while others are hardcorde div users.

Whatever your style is, Feedify got you covered by using classes on key elements.
Just make sure they're all here and you'll be good to go.

Note: Feedify is based on scrolling, so make sure you create enough items so there's something to scroll.

<pre><div class="feedify">
  <div class="feedify-item">
    <div class="feedify-item-header">
       This is the header of my item.
       It will remain stuck to top while scrolling.
    </div>
    <div class="feedify-item-body">
      This is the body of my item.
      I can put whatever I want in here.
    </div>
  </div>
</div></pre>

### Add some style

You're free to use the Feedify theme or not, but it still needs a few lines of CSS to work properly. Either include feedify.min.css in your page, or copy-paste the code in your own CSS stylesheet.

<pre>.feedify .feedify-item {
  position: relative;
}
.feedify .feedify-item .feedify-item-header {
  z-index: 100;
}
.feedify .feedify-item.fixed .feedify-item-header {
  position: fixed;
  top: 0;
}
.feedify .feedify-item.bottom .feedify-item-header {
  position: absolute;
  bottom: 0;
}</pre>

### Unleash the beast

Everything is set up, now you just need to pull the trigger. To fire Feedify, just add the following piece of code within a <script> tag in your page (or directly in your script page if you have one) and voilà!

<pre>$(function() {
  $('.feedify').feedify();
});</pre>

### Optional — Feedify theme

Feedify theme uses Bootstrap. You need to make sure you include at least version 3.3.4 of Bootstrap if you intend to use it.

<pre><link href="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.4/css/bootstrap.min.css" rel="stylesheet">
<link href="css/feedify.min.css" rel="stylesheet">
<link href="css/feedify-theme.min.css" rel="stylesheet"></pre>
