# Introduction #

SevenUp accepts options for customization in its test() function, as well as a callback to your own code after it fires (so you can run arbitrary code when IE6- is detected, on top of showing the overlay). Note that not all plugins support all features. It is up to the plugin designer to include these options when creating the lightboxHTML.

The options are explained below, but here is a full 'options' hash with every variable set to their defaults, to use as a quick reference:

```
var options = {
  enableClosing: true,
  enableQuitBuggingMe: true,
  overlayColor: "#000000",  
  lightboxColor: "#ffffff",
  borderColor: "#6699ff",
  downloadLink: osSupportsUpgrade ? 
                "http://www.microsoft.com/windows/internet-explorer" :
                "http://getfirefox.com",
  overrideLightbox: false,
  lightboxHTML: null,
  showToAllBrowsers: false
};

var callback = function() {
  // Switch IE-specific content
  // AJAX call to map IP to 'IE6 user' status
  // etc.
}

sevenup.test(options, callback);
```

# Details #

### enableClosing ###
By default, SevenUp allows the user to close the overlay window, for the "Support but Discourage" approach. But setting this to false disables that functionality, requiring IE7+.

### enableQuitBuggingMe ###
By default, SevenUp also allows the user to stop it from showing for a week, for your loyal but stubborn users. Setting this to false disables that functionality, making it so users see the upgrade reminder every time they view a page with SevenUp enabled.  It uses a cookie set to the domain "/" to remember users, so cookies must be enabled for this to work.

### overlayColor ###
When using the default SevenUp skin, the background overlay is #000000 by default, but can be whatever you like. When customizing, make sure you include the # if you're using hex. Keep in mind it will be shown at 80% opacity.

### lightboxColor ###
When using the default SevenUp skin, the lightbox is #ffffff by default, but can be whatever you like. This is effectively setting the 'background color' of the default skin's lightbox window.

### lightboxBorder ###
When using the default SevenUp skin, the border color is #6699ff by default, but can be whatever you like.

### downloadLink ###
By default, SevenUp checks the user's OS by looking at the browser's user-agent string. If their reported OS supports IE7+, its upgrade link goes to MSIE.  If not, it recommends Firefox.  If you want to customize which browser you recommend, but don't want to make your own skin, just set this option.

### overrideLightbox ###
Commonly used by plugins, this option works in concert with lightboxHTML to override SevenUp's default lightbox with the HTML provided in lightboxHTML.

### lightboxHTML ###
Commonly used by plugins. If overrideLightbox is set to true, SevenUp shows this HTML in place of its default.

### showToAllBrowsers ###
Great for debugging - if true, SevenUp fires for all browsers. If false (the default) only IE6- gets the notice.