

# HAVING vs WHERE
A HAVING clause is like a WHERE clause, but applies only to groups as a whole (that is, to the rows in the result set representing groups), whereas the WHERE clause applies to individual rows.

# How to make stored Procedures

- [javatpoint.com](https://www.javatpoint.com/stored-procedure-in-sql-server)

# What are the differences between PRIMARY, UNIQUE, INDEX and FULLTEXT when creating MySQL tables?

## Differences

 - **KEY** or **INDEX** refers to a normal non-unique index.  Non-distinct values for the index are allowed, so the index *may* contain rows with identical values in all columns of the index.  These indexes don't enforce any restraints on your data so they are used only for access - for quickly reaching certain ranges of records without scanning all records.

 - **UNIQUE** refers to an index where all rows of the index must be unique.  That is, the same row may not have identical non-NULL values for all columns in this index as another row.  As well as being used to quickly reach certain record ranges, UNIQUE indexes can be used to enforce restraints on data, because the database system does not allow the distinct values rule to be broken when inserting or updating data.

   Your database system may allow a UNIQUE index to be applied to columns which allow NULL values, in which case two rows are allowed to be identical if they both contain a NULL value (the rationale here is that NULL is considered not equal to itself).  Depending on your application, however, you *may* find this undesirable: if you wish to prevent this, you should disallow NULL values in the relevant columns.

 - **PRIMARY** acts exactly like a UNIQUE index, except that it is always named 'PRIMARY', and there may be only one on a table (and there *should* always be one; though some database systems don't enforce this).  A PRIMARY index is intended as a primary means to uniquely identify any row in the table, so unlike UNIQUE it should not be used on any columns which allow NULL values.  Your PRIMARY index should be on the smallest number of columns that are sufficient to uniquely identify a row.  Often, this is just one column containing a unique auto-incremented number, but if there is anything else that can uniquely identify a row, such as "countrycode" in a list of countries, you can use that instead.

   Some database systems (such as MySQL's InnoDB) will store a table's records on disk in the order in which they appear in the PRIMARY index.

 - **FULLTEXT** indexes are different from all of the above, and their behaviour differs significantly between database systems.  FULLTEXT indexes are only useful for full text searches done with the MATCH() / AGAINST() clause, unlike the above three - which are typically implemented internally using b-trees (allowing for selecting, sorting or ranges starting from left most column) or hash tables (allowing for selection starting from left most column).

   Where the other index types are general-purpose, a FULLTEXT index is specialised, in that it serves a narrow purpose: it's only used for a "full text search" feature.

## Similarities

 - All of these indexes may have more than one column in them.

 - With the exception of FULLTEXT, the column order is significant: for the index to be useful in a query, the query must use columns from the index starting from the left - it can't use just the second, third or fourth part of an index, unless it is also using the previous columns in the index to match static values.  (For a FULLTEXT index to be useful to a query, the query must use *all* columns of the index.)