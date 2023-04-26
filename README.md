# ff-chrome-folder

## Install my chrome folder mods

1. Enable Profile Customizations - in about:config @ `toolkit.legacyUserProfileCustomizations.stylesheets`

1. Now, in about:support, click on the ‘Open Directory’ and then create a folder named ‘chrome’ inside (if it doesn't exist).

1. Clone/copy this repo's contents into the newly created profile/chrome folder

1. Relaunch Firefox

<u>Note:</u> relaunching Firefox is required to apply any modifications made to the chrome folder

&nbsp;

## `userchrome.css`

<details>
<summary>my changes (topmost) + 4 different snippets copypasta'd</summary>

-   re-add panel title, but without "sidebar icon"
-   (fullscreen) undo clipping of location/toolbar
-   "expand" traffic button area (to reveal location bar reliably (w/ :hover))
-   (fullscreen) remove empty space
-   (fullscreen) sidebar window element - undo extra padding in #webext-panels-browser
-   sidebar window inner browser = set same bg as sidebery settings
-   (fix text collision) move sidebery panel title (if visible) to under/right of traffic button bar

#

</details>

-   add sidebar Compact Mode (animated collapse)
    [https://github.com/Graklinghunter/Hovertext-Css/blob/main/userChrome.css](https://github.com/Graklinghunter/Hovertext-Css/blob/main/userChrome.css)

-   add padding (arcfox)
    [https://github.com/use-arcfox/arcfox/blob/main/theme/userChrome.css](https://github.com/use-arcfox/arcfox/blob/main/theme/userChrome.css)

-   hide/show main toolbar when cursor over tabs toolbar, and whenever the focus is inside nav-bar (eg: Command+L)
    [https://github.com/MrOtherGuy/firefox-csshacks/tree/master/chrome/autohide_main_toolbar.css](https://github.com/MrOtherGuy/firefox-csshacks/tree/master/chrome/autohide_main_toolbar.css)

-   [firefox-vertical-tabs](https://github.com/ranmaru22/firefox-vertical-tabs)

## `userContent.css`

-   dark mode pdf viewer
-   higher contrast highlights (eg: matches in pdf find / regular find)

&nbsp;

<u>Note:</u> recommended (but not required) for use with [screenhook](https://github.com/steventheworker/screenhook) + a vertical tabs sidebar extension (I use [sidebery](https://github.com/steventheworker/sidebery))

<details>
  <summary>Why use screenhook? (macOS only)</summary>
&nbsp;

Firefox-specific screenhook features

-   left-edge of window = sidebar peak
-   top-edge of window = more consistent window - dragging (compensate for userChrome.css w/ auto-reveal location bar (prevents drag))
-   cmd+shift+T to reopen tabs AND windows (requires BTT bindings)

</details>
