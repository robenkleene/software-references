# macOS Troubleshooting

## Eject a Disk

For `The volume can't be ejected because it's currently in use.` error, use `sudo lsof /Volumes/<volume-name>` to see what's using the volume.

## Keyboard

- If the terminal (or other applications aren't receiving the `^␣` shortcut, it's because the `Select the previous input source` keyboard shortcut is swallowing it. Remove this shortcut under `Settings > Keyboard > Keyboard Shortcuts > Input Sources`.

## Garbled Audio

    sudo killall coreaudiod
