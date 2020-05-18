# Excel

## Keyboard Shortcuts

- `⇧⌘O`: Open recent
- `⇧␣`: Select row
- `⌃␣`: Select column
- `⌘A`: Select table
- `⇧⌃+`: Insert row (first select the row to avoid the Insert Cells dialog)
- `⇧⌃+`: Insert column (same shortcut as above?)
- `⌃U`: Edit current cell, when editing a cell, hit `⌘A` to switch to the formula bar (another option to edit in the formula bar is to turn off the "Edit Directly in Cell" preference, although this means you can never edit in the cell, even when not editing a formula)
- `⌘⌥v v ↩`: Paste values

## Navigation

- `^PgDn` / `^PgUp`: Go to next / previous worksheet

## Editing

- `⌃;`: Insert today's date
- `⇧⌃$`: Format cell as currency
- `⇧⌃%`: Format cell as percentage
- `⌃-`: Delete rows or columns
- `⌘K`: Edit shortcut
- `⌘A`: Jump between editing in the cell and in the formula bar
- `⌃A`: Select all in the formula bar
- `↩`: Stop editing and go the cell below
- `⇥`: Stop editing and go next cell
- `⌃↩`: Stop editing and stay in current cell
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

## Tips

- To resize all columns to fit, first click the special cell in the upper left where the row and column indexes meet, this should highlight the entire spreadsheet. While the whole spreadsheet is highlighted, clicking between columns as you would you normally resize a single column, will resize all columns.
- Select "Format > Column > AutoFit Selection" to auto-fit all rows
- To clear formatting, use "Edit" -> "Clear" -> "Formats"
- A more precise way to clear formatting is to open cell styles `⌘1` and select "Font" -> "Normal Font"
- Use "Paste" -> "Paste Values" to paste the results of a formula, rather than the formula itself.
- You can give a cell or a column a variable name (use "Formulas" -> "Define Name"), and then refer to it by name in formula.

## Transpose

To swap the orientation of rows and columns:

1. If you're using a Table, you need to convert it to a range first: "Table > Convert to Range"
2. Copy the cells, then select "Home > Paste > Transpose"

## Columns

### Re-Ordering Columns

1. First select the column with `^␣`. There are three possible selection states for a column, which determines what happens when the column is moved:

    1. *Just the cells are selected*, moving this will cause the moved cells to replace the cells that are moved to, preserving the headers.
    2. *The cells and header are selected*, moving this will move the column between another column.
	3. *The cells, header, and top label are selected*, moving this will replacing the headers and cells in another column.

	Hitting `^␣` will progress through these states in order, starting by just selecting the cells, unless header is selected, in which case the cells and data will be selected.
2. Hover over the column's border until a hand icon appears.
3. Drag the column to it's new location. Visual indication will determine which action will be performed:
	1. *A selection box appears around the destination cells with a cell range hover label* (e.g., `C2:C10`) appearing. This means the moved cells will replace the cells that are moved to.
	2. *A line appears between the destination columns with a cell range hover label* (e.g., `C2:C10`) appearing, this means the column will be moved between columns where the line appears.
	3. *A selection box appears around the destination cells with a cell column hover label* (e.g., `C:C`) appearing. This means the moved column will replace the column that is moved to.

## Cell Styles

Excel has some useful built-in styles under "Home" -> "Cell Styles".

- Normal
- Good
- Bad
- Neutral
- Input: Something meant to be changed
- Calculation: Something that is output

## Delimited Data

To add comma- or tab-delimited data, paste it into one cell, then select "Data" -> "Text to Columns"

1. Paste the data into one cell

## Fill Handle

Use the fill handle (little box to the bottom right of a selection box), to fill a bunch of cells with a pattern.

### Supported Lists

- Days of the week
- Dates
- Incremented or decremented numbers

## R1C1

R1C1 is Excel's "native" way of referencing cells. It can be helpful to switch to R1C1 mode (in "Preferences" -> "General" -> "Use R1C1 reference style" to see what's going on under the hood.

## Formula

- Use `⌘T` when editing a formula to switch between relative

### Symbols

- `&`: Concatenates
- `$`: Means absolute reference (as opposed to relative)
- `'`: Start the value of a cell with an apostrophe to make it plain text (e.g., to enter a number that starts with leading zeros)

