# macOS Settings

## Keyboard Shortcuts

- `⌃⌥␣` is bound by `Input Sources > Select next source in Input menu` by default, this binding should be disabled (Emacs uses this key to select the current s-expression for example)

## Dictation

- The default keyboard shortcut to show the enable dictation pop-up is `Press Control Key Twice`
- This can be set (or disabled) under `System Settings > Keyboard > Dictation > Shortcut`

## Accented Characters

- `Settings > Keyboard > Input Source > Other > Unicode Hex Input`

## Notes

- To turn off screenshot thumbnails, use `⇧⌘5`, then toggle off `Options > Show Floating Thumbnail`

## Defaults

Disable new window animations:

```
defaults write NSGlobalDomain NSAutomaticWindowAnimationsEnabled -bool NO
```

To enable key repeat (and disable press and hold for accents):

```
defaults write -g ApplePressAndHoldEnabled -bool false
```

Note that quitting and restarting apps is required after making this change.

## Focus

- Toggle off `Settings > Focus > Share across devices`, otherwise doing something like using a laptop on a train will cause constant `Driving` notifications
