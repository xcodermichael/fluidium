The initial Fluidium 0.1 release is based on the browser code powering both Fluid SSBs and Cruz (www.fluidapp.com, www.cruzapp.com). 

Almost all of the code included in this project was updated prior to this release, and some of it was rewritten completely. Stuff that was completely rewritten (and therefore may not be well-tested yet):

- FUDocumentController/FUDocument/FUWindowController/FUTabController/FUWindow : this is the code which handles basic browser window/tab management, and is the core functionality of the browser. It conforms to the Cocoa Document-based application design pattern.

- Userscripting : previously, Fluid and Cruz userscripting was based on GreaseKit. That has been removed and replaced with a new implementation in Fluidium.

- Browsa Plug-in


Stuff from Fluid/Cruz which is not currently included:

- Fluid.app (SSB creator/generator) : this codebase does not include the code for Fluid.app itself (the small application which can be used to create SSBs with a name/url/custom icon). Fluid.app itself represents a *very* small portion of the Fluid application. Most of the code is in the SSB Browser (and here in Fluidium).

- Thumbnail.fluidplugin : rewriting. will add soonish.

- Fullscreen : rewriting. will add soon.

- Custom window styles : I was using private apis which don't seem to be supported under 64-bit. This probably will not return any time soon. kinda dumb.

- MenuExtra SSB/Embedded SSB : this is cruft i wanted to remove. i might re-add these features by rewriting them. anyone is welcome to fork me and add this if they miss it, but for now, I don't :|

- short url expansion/creation : I will re-add this very soon.

- thumbnail-image-enhanced google search results : I will re-add this eventually.


Everything else from Fluid/Cruz is still included : Sparkle Software Update, Twitter Plugin, Browsa Plugin (web split views), Tabs Plugin (tab thumbnail images), userscripting, userstyles, shortcuts, window.fluid JavaScript object, Growl notifications, cocoa plugin architecture, URL whitelist/blacklists, basic bookmarks+bookmarks bar, basic browser history, custom user-agent strings.