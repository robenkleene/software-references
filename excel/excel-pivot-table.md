# Excel Pivot Table

## Basics

- **Create**: To create a Pivot Table, in the toolbar, select `Insert > Tables > PivotTable`.
- **Refresh**: To refresh a Pivotal Table, for example to update values or make a new field appear, right-click and select `Refresh`.

### More

- To **move** existing fields, drag the fields between "Filters", "Columns", "Rows", and "Values"
- To **delete existing fields**, drag the fields off of the Pivot Table sidebar
- Hide `Grand Total` row: `Design > Grand Totals > Off for Rows and Columns`
- You can change the formatting for cells  (`⌘1`) just like you would for regular cells (e.g., to display dates).

## Summarize

- **Sum:** The sum of the values (default)
- **Count:** The number of values, same as `COUNTA` (default for non-numbers)
- **Average:** The average of the values.
- **Max:** The largest value.
- **Min:** The smallest value.
- **Product:** The product of the values.
- **Count Numbers:** The number of values that are numbers, same as `COUNT`
- **StDev:** An estimate of the standard deviation of a population, where the sample is a subset of the entire population.
- **StDevp:** The standard deviation of a population, where the population is all of the values to be summarized.
- **Var:** An estimate of the variance of a population, where the sample is a subset of the entire population.
- **Varp:** The variance of a population, where the population is all of the values to be summarized.

## Errors

- To get around the "Pivot Table field name already exists" error when renaming a column to the same name as a column in an existing table, the convention is to add a space to the end of the column name.

### Hiding

Right-click the table and select "PivotTable Options...", then check "Display > Error values as:" and choose a default value.

### Naming Collusion

- "PivotTable field name already exists", if this matches a deleted column, you probably need to right-click and "Refresh" your table.
