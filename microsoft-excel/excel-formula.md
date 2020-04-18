# Excel Formulas

## Shortcuts

- `F9`: Evaluate and replace contents of a selected part of a formula
- `F2`: Switch between edit and formula mode when editing a cell

## Names

In a table, columns are automatically named by their headers. To name a table, do so under "Table" -> "Table Name:".

## Syntax

- `<>`: Not equal
- `$`: Is a locked reference, e.g., when the formula is cut & pasted, those cells will not change `=FORECAST.LINEAR([@Year],F2:F6,$A$2:$A$6)`

## Errors

- `#VALUE!`: Generic error
- `#NAME?`: A reference to another cell in your formula is invalid
- `#N/A`: Something can't be found or identified

### Handling

- `IFERROR`: Replace error with blank

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
