# OmniOutliner

## `.ooutline` Format

By default OmniOutliner's native file format, `.ooutline`, is a `flat file`, it can be changed to a `file package` under `Inspect > Document > Format and Metadata`

As a file package, the contents are stored as a `.xml` file with some additional metadata, this makes it a good candidate for storing files in source control.

## OPML

OmniOutliner can also read and write `.opml` files, but this disables rich text and linking to referenced files.
