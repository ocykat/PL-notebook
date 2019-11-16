# Oracle SQL

## Tools
* Database: Oracle Database Express Edition ver 18c.
* IDE: Oracle SQL Developer

## Terminology
* What is a schema? Check [here](https://asktom.oracle.com/pls/asktom/f?p=100:11:0::::P11_QUESTION_ID:6162110256950).

## Create Connection
### Create Common User
```
CREATE USER c##{username} IDENTIFIED BY {password};
```
### Grant Privileges To a User
```sql
GRANT ALL TO c##{username};
```

## Datatypes
### Character Datatypes
* `CHAR`: character values with fixed length. A `CHAR` datatype can have between 1 and 2,000 characters. If a length is not explicitly specified for a `CHAR`, it assumes the default length of 1.
* `VARCHAR2`: variable-length character strings. A length must be assigned to a `VARCHAR2`:  this length is the maximum length
for a value.
```sql
column VARCHAR(maxlength)
```
* `VARCHAR`: synonymous with the `VARCHAR2` datatype. However, you should use `VARCHAR2` instead of `VARCHAR`. More info [here](https://docs.oracle.com/cd/B28359_01/server.111/b28318/datatype.htm#i1835).
* `NCHAR`: similar to `CHAR`, but can store Unicode characters.
* `NVARCHAR2`: similar to `VARCHAR2`, but can store Unicode characters.

### Numeric Datatypes
* `NUMBER`: the only datatype that stores numeric values in Oracle.
  * Declaring a column or variable as `NUMBER` will automatically provide a precision of 38 digits.
  * `NUMBER` can also accept two qualifiers: precision and scale.
  * Usage:
```sql
column_name NUMBER                   /* default precision: 38 digits */
column_name NUMBER(precision, scale)
```

### Datetimes
The standard Oracle date format for input takes the form of `DD-MON-YY HH:MI:SS`, where:
* `DD` represents up to two digits for the day of the month.
* `MON` is a three-character abbreviation for the month.
* `YY` is a two-digit representation of the year.
* `HH`, `MI`, and `SS` are two-digit representations of hours, minutes, and seconds, re‐
spectively.
If you don’t specify any time values, their default values are all zeros in the internal storage.

### NULLs
`NULL` can be assigned as a value for any datatype.
None of the following conditions are true for Column A if the column contains a `NULL` value:
```sql
A > 0
A < 0
A = 0
A != 0
```
The presence of a `NULL` value can only be tested with the relational operator `IS NULL`.

## Create Table
