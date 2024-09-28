# Zen-bottombar
A theme for Zen Browser that moves the URL bar to the bottom of the user interface.

![Screenshot of interface with them theme enabled.](https://github.com/sprokolopolis/Zen-bottombar/blob/main/bottombar.png)

## How to set it up:
* Navigate to `about:profiles` in the url bar.
* In the section of your active profile, in the Root Directory row, press "Open Folder"/"Show in Finder").
* It should open your file explorer and show you a highlighted folder. Open that folder and then open the "chrome" folder in there.
* Place both `userChrome.css` and `bottombar.css` in the chrome folder.
* In Zen Browser, navigate to about:config in your url bar.
* Type: `toolkit.legacyUserProfileCustomizations.stylesheets` and set to true.
* Type: `uc.bottom.bar` and set to true.
* Type: `svg.context-properties.content.enabled` and set to true.
* Restart Zen

## Current Issues:
* The background of the URL bar is not the exact color as the rest of the UI (sidebar, etc). I'm not sure if there is layering of multiple transparent backgrounds or if I am just not using the right color variable.
* The width of the URL bar is set to `width: calc(100% - 184px);`. The 184px  is mant to make up for the sidebar width displacement. Without it, the bar elements will go out of bounds. The 184px isn't exact, depending on how wide your sidebar is. Originally, I used a more complicated calc() function with the variables icons sizs/padding, but it just wasn't being intepreted properly.
* Might not work in compact mode.
