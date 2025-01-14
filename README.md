<h1 align="center">
  <img width="120" height="120" src="https://github.com/greeeen-dev/natsumi-browser/blob/main/images/icon.png?raw=true">
  <br>
  Natsumi Browser
</h1>

<p align="center">A skin for Zen Browser that makes things <strong><i>~flow~</i></strong>.</p>

![](https://github.com/greeeen-dev/natsumi-browser/blob/dev/images/natsumi-preview-3.png?raw=true)

## What is Natsumi Browser?
Natsumi Browser (or Natsumi, for short) is a skin made for [Zen Browser](https://zen-browser.app)
that adds lots of polish to the design by incorporating animations, blurs and more. It's pretty much
the skin I personally use, but made public because people wanted the CSS.

Natsumi is NOT a standalone browser. I don't even intend on making one.

Natsumi has been tested on `1.0.2-b.3` (Beta) and `1.0.2-t.4 2024-12-19` (Twilight).

## Features
### Polished look
Natsumi Browser's looks are based on asev's [ZenCss](https://github.com/lunar-os/ZenCss), with some
additional tweaks and patches added on top to create a beautiful and polished experience.

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/interface.gif?raw=true)

### Natsumi URLbar
With Natsumi URLbar, Natsumi gives the expanded URLbar a completely fresh new look, so it feels very
cozy while also having lots of room for search suggestions.

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/natsumi-urlbar.gif?raw=true)

### Natsumi Findbar
Say hello to Natsumi Findbar! Natsumi Findbar shares a similar design as Natsumi URLbar, bringing you
the same cozy and modern experience. Inspired by [RobotoSkunk](https://github.com/RobotoSkunk)'s [Better
Find Bar](https://zen-browser.app/mods/a6335949-4465-4b71-926c-4a52d34bc9c0/) Mod.

![](https://github.com/greeeen-dev/natsumi-browser/blob/dev/images/findbar.png?raw=true)

### Tab Groups
Natsumi Browser uses a customized version of [vicky5124](https://github.com/vicky5124)'s CSS for Tab
Groups. Group away to keep things organized!

![](https://github.com/greeeen-dev/natsumi-browser/blob/main/images/tab-groups.gif?raw=true)

### Natsumi PDF Viewer
Send your PDF viewer to the 21st century! Natsumi Browser Pages includes tweaks for the default PDF
viewer, giving it the modern look it really deserves.

![](https://github.com/greeeen-dev/natsumi-browser/blob/dev/images/natsumi-pdf.png?raw=true)

## Installation
This skin is not available on the Zen Mods page, as this isn't intended to be a Mod. You will need to
install it by copying the files to your profile's chrome folder.

### Natsumi Browser
#### If you already have a userChrome.css file
1. Copy natsumi-config.css and natsumi folder to your chrome folder.
2. Add `@import "natsumi/natsumi.css";` to the beginning of your userChrome.css file.
3. Restart Zen Browser and enjoy!

#### If you don't have a userChrome.css file
1. Create a new chrome folder in your profile folder, if you haven't already.
   ([guide](https://docs.zen-browser.app/guides/live-editing))
2. Copy userChrome.css to the chrome folder.
3. Copy natsumi-config.css and natsumi folder to the chrome folder.
4. Restart Zen Browser and enjoy!

### Natsumi Browser Pages
#### If you already have a userContent.css file
1. Add `@import "natsumi-pages/natsumi-pages.css";` to the beginning of your userContent.css file.
2. Restart Zen Browser and enjoy!

#### If you don't have a userContent.css file
1. Create a new chrome folder in your profile folder, if you haven't already.
   ([guide](https://docs.zen-browser.app/guides/live-editing))
2. Copy userContent.css to the chrome folder.
3. Copy natsumi-config.css to the chrome folder, if you haven't already.
4. Copy natsumi-pages folder to the chrome folder.
5. Restart Zen Browser and enjoy!

## Browser configs (in about:config)
These are the configs you can use to tweak Natsumi Browser. If you want to tweak the animation duration
and delay, change the variables in the config.css file.

### Base theme
- `natsumi.theme.clip-path-force-polygon`: Uses polygon instead of inset for URLbar and Zen Sidebar
  blurring. Enable this if you need this for compatibility with other userchromes/Mods like
  [Cohesion](https://github.com/TheBigWazz/ZenThemes/tree/main/Cohesion).
- `natsumi.theme.disable-blur`: Disables blurring for glass effects. Use this if Zen Browser lags
  too much.
- `natsumi.theme.disable-glass-shadow`: Disables shadow for glass effects.
- `natsumi.theme.disable-loading-animations`: Disables loading animation for tabs.
- `natsumi.theme.disable-urlbar-animation`: Disables URLbar loading animation for tabs.
- `natsumi.theme.enable-border-animation`: Enables border loading animation for tabs. This may use up
  quite some GPU.
- `natsumi.theme.fullscreen-glass-effect`: Enables glass effect for full screen popup message.

### URLbar
- `natsumi.urlbar.disabled`: Disables Natsumi URLbar and reverts the URLbar style back.
- `natsumi.urlbar.disable-transparency`: Disables URLbar background transparency.
- `natsumi.urlbar.force-nowrap`: Prevents wrapping to make things more compact regardless of window
  width.
- `natsumi.urlbar.light`: Disables some animations to make Natsumi URLbar lighter.

### Navbar
- `natsumi.navbar.floating-navbar`: Makes the navbar float on compact mode.
- `natsumi.navbar.glass-effect`: Adds glass effect for the navbar on compact mode.

### Sidebar
- `natsumi.sidebar.blur-zen-sidebar`: Blurs Zen Sidebar background. This may cause some lag when you
  have both Zen Sidebar and Natsumi URLbar opened at the same time.
- `natsumi.sidebar.containers-dashed-border`: Uses dashed border for container tabs instead of solid
  border. Selected tabs will always use solid border.
- `natsumi.sidebar.containers-thicker-gradient`: Makes container tabs indicator gradient "thicker".
- `natsumi.sidebar.containers-no-inactive-border`: Hides the container tabs indicator border when the
  tab is not selected.
- `natsumi.sidebar.disable-bigger-tab-label`: Disables bigger tab labels and reverts them back to the
  normal font size.
- `natsumi.sidebar.disable-panel-transparency`: Disables transparent background for sidebar panels
  (e.g. Bookmarks).
- `natsumi.sidebar.enable-tab-groups`: Enables Tab Groups CSS. This is opt-in as the developer does
  not recommend using custom CSS to implement Tab Groups at the moment.
- `natsumi.sidebar.floating-panel`: Makes the Firefox sidebar panel float.
- `natsumi.sidebar.panel-glass-effect`: Adds glass effect to Firefox sidebar panel.
- `natsumi.sidebar.panel-position-center`: Vertically centers Firefox sidebar panel if it is floating.
- `natsumi.sidebar.panel-position-bottom`: Moves Firefox sidebar panel to the bottom if it is floating.
  Overrides `natsumi.sidebar.panel-position-center` if enabled.
- `natsumi.sidebar.panel-position-right`: Moves the Firefox sidebar panel to the right if it is floating.
- `natsumi.sidebar.panel-resizable`: Makes the Firefox sidebar panel resizable.
- `natsumi.sidebar.right-gradient`: Moves tabs and containers indicator gradients to the right.
- `natsumi.sidebar.tabs-glass-effect`: Adds glass effect for the sidebar on compact mode.
- `natsumi.sidebar.unlimited-pinned-tabs`: Removes the limit on the maximum number of tabs being shown
  in the pinned section of the vertical tabs.
- `natsumi.sidebar.zen-sidebar-glass-effect`: Adds glass effect to Zen Sidebar.

### Findbar
- `natsumi.findbar.disabled`: Disables Natsumi Findbar and reverts the findbar style back.
- `natsumi.findbar.disable-not-found-bg`: Disables red background that appears when there are no
  results.
- `natsumi.findbar.wider-findbar`: Increases maximum Findbar width back to 720px.

### PDF Viewer
- `natsumi.pdfjs.disabled`: Disables Natsumi PDF Viewer and reverts the PDF viewer back.

### Misc
- `natsumi.debug.legacy`: Enables support for 1.0.2-b.0 and 1.0.2-b.1.

## FAQs
### "Mod xyz has a similar look as Natsumi, did they copy you?"
Like I've said in the Features section, Natsumi's base UI CSS comes from asev's ZenCss repository.
This is actually a very popular userchrome among the Zen Browser community, so it's likely that the
Mod also uses the same userchrome I used.

### "Can I use other userchromes with Natsumi?"
Sure! Just paste it right below the Natsumi Browser loader (userChrome.css) and you can use your own
userchrome alongside Natsumi Browser.

### "Can I disable individual features?"
You're free to disable loading certain modules (CSS files) if you feel like it. But you will still need
to load config.css, natsumi/preload.css and natsumi/postload.css for things to work.

### "Why is userChrome.css so empty?"
Natsumi Browser uses a system where the userChrome.css file acts as a loader that loads the skin,
instead of being the file that contains all rules. This way, it's easier for users to quickly enable and
disable custom CSS.

## Troubleshooting
### "URLbar blur won't work!"
Make sure both `layout.css.backdrop-filter.enabled` and `layout.css.backdrop-filter.force-enabled` are
set to true. Also make sure that you're using WebRender and hardware rendering.

### "Zen Browser lags a lot!"
This may be due to the URLbar blurring or animations (likely the blur). Set `natsumi.theme.disable-blur`
to false to disable the blur, and `natsumi.urlbar.light` to true to disable the animations.

### "I don't see any of the Natsumi options in about:config!"
These are custom options which you need to create. Type in the exact name, then press the plus button on
the right to create the config.

### "Tab groups aren't working!"
> [!WARNING]
> The developer of Zen Browser recommends **against** using custom CSS to implement Tab Groups like
> Natsumi's for the time being. Proceed at your own risk.

Set `browser.tabs.groups.enabled` and `natsumi.sidebar.enable-tab-groups` to true.

### "Something's bugged!"
There may be Zen Mods or userchromes that you're using alongside Natsumi Browser that breaks things.
Please disable these then try again.

If the issue still persists, open an issue or report the bug to the developer through Discord.

## Acknowledgements
Thank you to:
- [asev](https://github.com/lunar-os) for ZenCss, which serves as the base for Natsumi Browser's base
  CSS, and the tab appear animation
- [vicky5124](https://github.com/vicky5124) for the Tab Groups CSS
- [mr-cheff](https://github.com/mr-cheff) and Zen's
  [contributors](https://github.com/zen-browser/desktop/graphs/contributors) for creating Zen Browser
