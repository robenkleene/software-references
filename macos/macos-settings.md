# macOS Settings

- To turn off screenshot thumbnails, use `⇧⌘5`, then toggle off `Options > Show Floating Thumbnail`

## Defaults

Disable new window animations:

    defaults write NSGlobalDomain NSAutomaticWindowAnimationsEnabled -bool NO

To enable key repeat (and disable press and hold for accents):

    defaults write -g ApplePressAndHoldEnabled -bool false

Note that quitting and restarting apps is required after making this change.
