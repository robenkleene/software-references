# Google Chrome DevTools

- `⌘]` / `⌘[`: Next / previous panel
- `⌘⌥J`: Toggle console
- `⌘⌥C`: Inspect element (this can be used to bring focus back to Elements in the DevTools)
- `⎋`: Toggle drawer
- `⌘⇧D`: Switch docking position
- `⌘⇧M`: Toggle responsive mode
- `^backtick`: Focus drawer (can be used even when web page content has focus)
- `⇧⌘P`: Bring up a fuzzy search panel to jump to various DevTools (this can be used to bring focus back to the DevTools)

## CSS

- When a numerical CSS value is selected in the `Styles` tab, you can increment and decrement it by scrolling (two-finger dragging) up and down.

## Tips

- Right-click and element and select "Copy styles" to copy all of the CSS styles applied to an element.

## Notes

- Source Maps are used by the DevTools to map a pre-processed file to a file on disk, e.g., a TypeScript file. Source Maps can be accessed in the `Sources` tab of the DevTools.

The problem is probably here:

```
for (var i = 0; i < testFilePaths.length; i++) {
  var testFilePath = testFilePaths[i];
  var spawnArgs = [testFilePath].concat(args);
  var spawn = require('child_process').spawnSync;
  spawn('mocha-phantomjs', spawnArgs, { stdio: 'inherit'});
}
```

I don't think we have a `mocha-phantomjs` binary installed?

## Troubleshooting

To exit responsive design mode, use `⌘⇧M`.
