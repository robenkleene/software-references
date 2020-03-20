# Excel Formulas

## Join

Get the index:

	=MATCH([@ID],Startups[ID],0)

The `0` forces an exact match.

	=INDEX(Startups,MATCH([@ID],Startups[ID],0),2)

The `2` is the index offset of the value you're looking for.

## Names

In a table, columns are automatically named by their headers. To name a table, do so under "Table" -> "Table Name:".
