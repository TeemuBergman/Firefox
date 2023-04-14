# Firefox customization

![](.\images\screenshot.png)

Just a few quick tweaks to Firefox's UI to make it more compact by sacrificing few usability elements. This customization is mostly intended to be used in Windows 11 with dark theme.

### Install instructions

1. Find your `Profile Folder` location: main menu >> Help >> More troubleshooting information
2. In row `Profile Folder` click `Open Folder`
3. Paste the cloned `chrome` folder in to your `Profile Folder` 
4. Open `about:config` and set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`
5. Restart Firefox

### Requirements

This customization removes all close tab and close window buttons, so user is required to know basic Firefox keyboard shortcuts i.e.: `ctrl+w` to close a tab and `ctrl+shift+w` to close a window. In `about:config` user can also set `browser.tabs.closeTabByDblclick` to `true` to close tabs by double clicking on them.

### Pro tip - updateability

If you use Git and want to clone this project locally, in Windows you can create a `directory junction` from root of this cloned project folder to root of your Firefox profile folder using mklink:

```
mklink /J "root-of-your-firefox-profile" "root-of-this-project/chrome"
```

This way updating customization files is easier by using `git pull` from the cloned project folder.