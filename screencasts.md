# Screencasts

Recording screencasts with QuickTime and editing in After Effects.

## Recording in QuickTime

Open QuickTime, select "File > New Screen Recording" (`⌃⌘N`), record then trim and save.

Or just use `⇧⌘5`.

## Edit in After Effects

1. Make a new composition `1080x720`. (Set "Editing Mode: `HDV 1080p`"
2. Save the project in a new directory, and drag your footage into that directory
3. Drag your footage into the composition
4. Hold shift and drag to resize the footage to the right size

## Material

### `git`

Demonstrating anything with `git` can be hard because you might not have a commit checked out to look at. An easy way to quick setup an environment where you can simulate a working directory with changes is to run the following commands:

    git checkout <rev>~1
    git show <rev> | git apply

What this does is go to a commit, and then revert that current commit, but only in the working tree. This simulates being in the situation of about to apply that commit.

