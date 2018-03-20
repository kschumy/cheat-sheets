# Active Record

## Migrations

### Steps for Migration
1. Create a model  
- `rails generate model  title:string author:string`
2. Generate a migration

### most common methods you'll encounter in migrations
  - `create_table(table_name)`: Creates a new table in the database, this is the command that the first migration used.
  - `add_column(table_name, column_name, data_type, options)`: Adds a column to an existing table.
  - `remove_column(table_name, column_name)`: Removes a column from an existing table.
  - `change_column(table_name, column_name, new_data_type)`: Changes an existing column from one data type to another.
  - `rename_column(table_name, old_column, new_column)`: Renames a column to match the newly given column name.
  
  ## Naming Conventions
 _model_ class and file names are singular  
 associated database table is pluralized The idea is that the table is _all the students_, while an __instance__ of the _model_ describes just one student. Here's a handy table:

|Model / Class (singular) | Table / Schema (plural)| Filename (singular) |
|:-----------------------:|:----------------------:|:-------------------:|
| Book                    | books                  | book.rb             |
| Post                    | posts                  | post.rb             |
| LineItem                | line_items             | line_item.rb        |
| Mouse                   | mice                   | mouse.rb            |
| Medium                  | media                  | medium.rb           |
| Person                  | people                 | person.rb           |
| Deer                    | deers                  | deer.rb             |
