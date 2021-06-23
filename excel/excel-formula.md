# Excel Formulas

## Shortcuts

- Use `⌘T` when editing a formula to switch between relative
- `F9`: Replace cell references with values (e.g., replace `H6:J6` with `{10,20,30}`)
- `F2`: Switch between edit and formula mode when editing a cell, in enter mode, you can select cells with the keyboard. (Whether the mode is currently "Enter" or "Edit" is shown in the lower left of the window)
- `F4`: Toggle between absolute and relative references (e.g., insert `$`). Hitting this repeatedly rotates between absolute, absolute row, absolute column, and relative.

## Text Editing

When editing formula, the usual text editing shortcuts are not available:

- `⌘←` / `⌘→`, `⌥←` / `⌥→`: Move by word
- `HOME`: Beginning of forumla
- `END`: End of forumla

### Tips

- Double-click a value then select cells to replace that value.
- When editing a function in a formula, a bar appears below the cell with the function signature, clicking the arguments in that function signature select that argument.
- Windows Excel has a "Formula > Evaluate Formula" button that lets you step through formula, this button isn't in the Mac version.

## Names

In a table, columns are automatically named by their headers. To name a table, do so under "Table" -> "Table Name:".

## Arrays

Array syntax is `{10,20,30}`, e.g., cell references like `H6:J6` return this.

(It appears `{10;20;30}` is also valid syntax.)

## Syntax

- `<>`: Not equal
- `$`: Is a locked reference, e.g., when the formula is cut & pasted, those cells will not change `=FORECAST.LINEAR([@Year],F2:F6,$A$2:$A$6)`(absolute reference as opposed to relative)
- `&`: Concatenates
- `'`: Start the value of a cell with an apostrophe to make it plain text (e.g., to enter a number that starts with leading zeros)

## Errors

- `#VALUE!`: Generic error
- `#NAME?`: A reference to another cell in your formula is invalid
- `#N/A`: Something can't be found or identified

### Handling

- `IFERROR`: Replace error with blank
- `=IF(ISERR(D3),IF(ERROR.TYPE(D3)=2,0,NA()),D3)`: Return different values based on error type

## Functions

- `=FORECAST.LINEAR(x, known_y’s, known_x’s)`: `=FORECAST.LINEAR([@Year],B2:B6,A2:A6)`

### Join

Get the index:

    =MATCH([@ID],Startups[ID],0)

The `0` forces an exact match.

    =INDEX(Startups,MATCH([@ID],Startups[ID],0),2)

The `2` is the index offset of the value you're looking for.

### Sum

Use an `ID` to get the sum of rows in a different column:

    =SUMIF(Funding[ID], [@ID], Funding[Amount])

`Funding[ID]` Get the list of `ID` from the `Funding` column, `[@ID]` test if matches the `ID` in this column, `Funding[Amount]` sum all the `Amount` values that match in the `Funding` table.

## Examples

- `=DATEDIF([@[2.0]], [@[3.0]], "D")`: Show duration in days

## `VLOOKUP`

    VLOOKUP (lookup_value, table_array, col_index_num, [range_lookup])

- `lookup_value`: The value used as a key
- `table_array`: Where to get the value from
- `col_index_num`: Offset from the key to column with the value
- `range_lookup`: Boolean for whether to use an exact match

### Tips

- You can click between sheets to reference tables in other sheets

### Example

    =VLOOKUP([@Date],Table6,2,FALSE)

Use the date from this table `[@Date]` to get the value that is `2` columns from the key in `Table6`.


## `AGGREGATE`

`AGGREGATE` is a quick way to perform a calculation while ignoring errors, e.g., this averages values from `VLOOKUP` ignoring `#N/A`.

    =AGGREGATE(1, 6, VLOOKUP([@Date],OneStat,2,FALSE), VLOOKUP([@Date],TheCounter,2,FALSE))

Note oddly `AGGREGATE` does not support arrays, e.g., `=AGGREGATE(1,6,{10,20,30})` returns a `#VALUE!` error.
