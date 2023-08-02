# Firefox Settings

## Advanced

At the `about:config` URL.

- `browser.tabs.insertAfterCurrent`: The new tab shortcut opens in the current tab instead of at the far right
    - There's a related option, `browser.tabs.insertRelatedAfterCurrent`, that affects `⌘click` links, but it's `true` by default
- `browser.link.open_newwindow: 2`: Open links to in new window instead of tabs
- `browser.altClickSave`: Allow download by `MMB` clicking
- `accessibility.typeaheadfind`: Search as you type - `browser.tabs.insertAfterCurrent`: Insert new tab to the right of current tab *Turning this off for now, it creates more tab management because if you want to quickly make a new search on the same topic, the tab for that search should be appended to the end, not inserted in the middle*
- `accessibility.typeaheadfind.manual`: Set to false to disable the `/` shortcut that interferes with website shortcuts to focus search bars
- `browser.gesture.swipe.left`: `cmd_scrollLeft` disable left swipe
- `browser.gesture.swipe.right`: `cmd_scrollRight` disable right swipe
## Settings

- To get rid of the search icons that show up at the bottom of the address bar, untick all the search engines under `Search Shortcuts` in settings
- Disable `Preferences > History > Remember search and form history` because it interferes with website's built-in autocomplete
- Turn off `Address Bar -- Firefox Suggest > Open tabs`

## Enhanced Tracking Protection

- To disable for a site, click the shield icon to the left of the URL and toggle it off

## Google Earth View

To set Google Earth View for new windows as well as new tabs, in `Preferences`, under `Homepage and newwindows`, click set `Custom URLs...` then choose `Use Current Page`, with just a tab showing a Google Earth preview visible.
