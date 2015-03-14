<table cellpadding='5'><tr><td valign='top'>

<h2>Help rid the world of IE6 with one line of javascript!</h2>

Easily require (or just encourage) IE versions 7 and up with this extremely small javascript include. (Users of non-IE browsers are unaffected.)<br>
<br>
Include one small JS file in the header of your page, and call the testing function. (Usually in your body.onload function, but anywhere works) Like so:<br>
<br>
<pre><code>&lt;script type="text/javascript" src="sevenup.0.3.min.js"&gt;&lt;/script&gt;<br>
...<br>
&lt;body onload="sevenUp.test( options, callback );"&gt;<br>
</code></pre>

And you're done! OR to use the black plugin, the code looks like so:<br>
<br>
<pre><code>&lt;script type="text/javascript" src="sevenup.0.3.min.js"&gt;&lt;/script&gt;<br>
&lt;script type="text/javascript" src="sevenup_black.0.3.min.js"&gt;&lt;/script&gt;<br>
...<br>
&lt;body onload="sevenUp.plugin.black.test( options, callback );"&gt;<br>
</code></pre>

OR create your own plugin with nothing but basic HTML/CSS knowledge, and a little copy/paste! Check out the file 'sevenup_pluginexample.0.3.js', rename it to your plugin name, and fill in your HTML!<br>
<br>
<font color='red'>
<b>Edit 4/28:</b> Documentation on settings options is up! Thx for everybody's patience :) <a href='http://code.google.com/p/sevenup/wiki/Customization'>http://code.google.com/p/sevenup/wiki/Customization</a>
</font>

Here's how it works right now: When viewed in IE6 or older, a pure-CSS lightbox pops up, suggesting that the user upgrade their outdated web browser. When NOT viewed in IE6/older, the user has no idea the script is there. You can either require the upgrade, or let them through with a warning.<br>
<br>
<h2>Features</h2>
<ul><li>SIMPLE: Just a 1K file, and one line both includes & activates the lightbox.<br>
</li><li>FLEXIBLE: You can force upgrades or allow users to continue on to the site's content.<br>
</li><li>INFORMATIVE: Explains in plain terms WHY they should WANT to upgrade.<br>
</li><li>CUSTOMIZABLE: Easily match your site's color scheme.<br>
</li><li>FORGIVING: "Stop bugging me" feature for loyal but stubborn users.</li></ul>

<h2>Features on the Way</h2>
<ul><li>Improved default CSS<br>
</li><li>Improved browser detection<br>
</li><li>Themes! Above and beyond the already-easy color customization.<br>
</li><li>Your idea? Find me at <a href='http://twitter.com/staringispolite'>http://twitter.com/staringispolite</a></li></ul>

<h2>More about the Movement</h2>
This project was inspired by...<br>
<ul><li>Google's effort (<a href='http://tinyurl.com/c83443'>http://tinyurl.com/c83443</a>),<br>
</li><li>A growing movement started in Norway (<a href='http://bit.ly/vIkw'>http://bit.ly/vIkw</a>), and<br>
</li><li>My general hatred for that browser we all know so, so well<br>
</td><td valign='top'>
<img src='http://sevenup.googlecode.com/files/sevenup_plugin_black.jpg' /></li></ul>

SevenUp triggered in IE6, with the "black" plugin. (out now! downloads section)<br>
<br>
<img src='http://sevenup.googlecode.com/files/SevenUp_0.2_Triggered_IE6.png' />

SevenUp in action in IE6, no plugins<br>
</td></tr></table>

<p>
If you liked this, check out more projects from me (<a href='http://staringispolite.com'>Jonathan Howard</a>) - in 2010 I'll be maintaining this project much more than previously, and releasing others as well.<br>
</p>
<p>
For instance: Enjoy Python, but tired of people telling you how to type to /your/ computer? Check out <a href='http://www.staringispolite.com/likepython'>Like, Python</a> and code like the kids are typing these days :)<br>
</p>