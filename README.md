
PL/SQL script to create sequence and trigger for primary key columns
Purpose
The purpose of this script is to create a sequence and trigger for each primary key column in the Oracle database tables whose data type is NUMBER.

How it works
The script declares a cursor named table_cursor that selects the table name and column name of each primary key column whose data type is NUMBER. It then loops through each row in the cursor, drops the existing sequence (if any) with the name Table_Name_seq, creates a new sequence with the same name, and sets the starting value of the sequence to the maximum value of the primary key column plus 1. It also creates a trigger for each table that automatically assigns the sequence value to the primary key column of any new record that is inserted.

Prerequisites
This script assumes that you have a set of tables with primary key columns whose data type is NUMBER.

How to use
To use this script, simply run it in your Oracle database. The script will create a new sequence and trigger for each primary key column in the tables that meet the specified criteria.

Disclaimer
This script is provided as-is, without any warranty or support. Use it at your own risk.

![out_1](https://github.com/AyaMedhat555/Pl_SQL/assets/63666107/291a33c2-4162-4f11-9c37-cedd1898bae1)

