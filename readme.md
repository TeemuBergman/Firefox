# Firefox customization

Just a few quick tweaks to Firefox's UI. This customization is mostly intended to be used in Windows 11 with dark theme.

### Install instructions

1. Find your `Profile Folder` location: main menu >> Help >> More troubleshooting information
2. In row `Profile Folder` click `Open Folder`
3. Paste the cloned `chrome` folder in to your `Profile Folder` 
4. Restart Firefox
5. ???
6. Profit!

### Pro tip

In Windows you can create 'a hard link' from local clone to your Firefox profile folder:

```
mklink /J "location-of-your-firefox-profile" "location-of-this-project"
```