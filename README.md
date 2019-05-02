# sqlanywhere-formatnumber

**Formats a number as a German currency value in SAP SQL Anywhere**

This functions takes a number in an SQL Anywhere database and formats it like a German currency value.

- number value is rounded to 2 decimal places
- comma as decimal delimiter
- point as thousand separator
- NO currency sign!

## Examples

```sql
SELECT dba.FormatNumber(12);                -- 12,00
SELECT dba.FormatNumber(12.5725);           -- 12,57
SELECT dba.FormatNumber(100624.958750);     -- 100.624,96
```


## Source

I've taken this example from [Volker Barth's post to the SQL Anywhere forum here](https://sqlanywhere-forum.sap.com/questions/1520/how-do-i-format-numbers-in-sqla) and reformatted it to my own needs.
