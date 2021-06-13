# Excel

## Keyboard Shortcuts

- `⌘1`: Format cells
- `⇧⌘O`: Open recent
- `⇧␣`: Select row
- `⌃␣`: Select column
- `⌘A`: Select table
- `⇧⌫`: Clear selection
- `⇧⌃+`: Insert row (first select the row to avoid the Insert Cells dialog)
- `⇧⌃+`: Insert column (same shortcut as above?)
- `⌘⌥v v ↩`: Paste values
- `⇧F10`: Open right-click menu
- `⌃F2`: Focus menubar
- `⌘⌥R`: Toggle ribbon
- `F6`: Focus ribbon (this is practically useless)
- `⇧⌘R`: Sort

## Navigation

- `^PgDn` / `^PgUp`, `⌥←` / `⌥→`: Go to next / previous worksheet

## Editing

- `⌃U`: Edit current cell, when editing a cell
- `⌃;`: Insert today's date
- `⌘;`: Insert current time
- `⌃-`: Delete rows or columns
- `⌘K`: Edit link
- `⌘A`: Jump between editing in the cell and in the formula bar (another option to edit in the formula bar is to turn off the "Edit Directly in Cell" preference, although this means you can never edit in the cell, even when not editing a formula)
- `⌃A`: Select all in the formula bar
- `↩`: Stop editing and go the cell below
- `⇥`: Stop editing and go next cell
- `⌃↩` or `⌘↩`: Stop editing and stay in current cell
- `⌥↩`: Enter multiple lines of text

## Selection

When a group of cells are selected.

- `⌃D`: Fill down
- `⌃⌘V`: Paste special, e.g., to add or multiply all cells by the value on the clipboard

## Cell Editing

Editing a cell when there's a selection.

- `⌃↩`: Fill all selected cells with the same value
- `⇥`: Edit the next selected cell.
- To insert a link, enter the link text, finish editing the cell, and choose "Insert > Link"

## Transpose

To swap the orientation of rows and columns:

1. If you're using a Table, you need to convert it to a range first: "Table > Convert to Range"
2. Copy the cells, then select "Home > Paste > Transpose"

## Columns

### Re-Ordering Columns in a Table

- If the data is not in a table, select the column with `^␣` and hold `⇧` while dragging the edge of the column (the cursor should change to a hand icon).

#### Tables

Note that this method will only work for tables.

1. First select the column with `^␣`. There are three possible selection states for a column, which determines what happens when the column is moved:

   1. _Just the cells are selected_, moving this will cause the moved cells to replace the cells that are moved to, preserving the headers.
   1. _The cells and header are selected_, moving this will move the column between another column.
   1. _The cells, header, and top label are selected_, moving this will replacing the headers and cells in another column.

   If it's a table, hitting `^␣` will progress through these states in order, starting by just selecting the cells, unless header is selected, in which case the cells and data will be selected.

2. Hover over the column's border until a hand icon appears.
3. Drag the column to it's new location. Visual indication will determine which action will be performed:
   1. _A selection box appears around the destination cells with a cell range hover label_ (e.g., `C2:C10`) appearing. This means the moved cells will replace the cells that are moved to.
   2. _A line appears between the destination columns with a cell range hover label_ (e.g., `C2:C10`) appearing, this means the column will be moved between columns where the line appears.
   3. _A selection box appears around the destination cells with a cell column hover label_ (e.g., `C:C`) appearing. This means the moved column will replace the column that is moved to.

## Delimited Data

To add comma- or tab-delimited data, paste it into one cell, then select "Data" -> "Text to Columns"

1. Paste the data into one cell

## Fill Handle

Use the `Fill Handle` (little box to the bottom right of a selection box), to fill a bunch of cells with a pattern.

- To see more options, use `RMB` instead of `LMB` when dragging out the `Fill Handle`, the menu will show up when the mouse button is released.

### Supported Lists

- Days of the week
- Dates (there are options for this like weekdays, months, and years when using `RMB`)
- Incremented or decremented numbers

## R1C1

R1C1 is Excel's "native" way of referencing cells. It can be helpful to switch to R1C1 mode (in "Preferences" -> "General" -> "Use R1C1 reference style" to see what's going on under the hood.

## Tips

- Excel in OneDrive is superior to just using iCloud Drive, OneDrive allows live-collaborative editing, if you have a file open and edit it on another device, files hosted in OneDrive will show those edits live.
- To resize all columns to fit, first click the special cell in the upper left where the row and column indexes meet, this should highlight the entire spreadsheet. While the whole spreadsheet is highlighted, clicking between columns as you would you normally resize a single column, will resize all columns.
- Select "Format > Column > AutoFit Selection" to auto-fit all rows
- Use "Paste" -> "Paste Values" to paste the results of a formula, rather than the formula itself.
- You can give a cell or a column a variable name (use "Formulas" -> "Define Name"), and then refer to it by name in formula.
