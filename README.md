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


