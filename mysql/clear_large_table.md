# Clear out a large table with minimial locking

```sql
# Create a new table with the same structure
create table the_table_new like the_table;

# Rename both tables. This is atomic.
rename table the_table to the_table_old, the_table_new to the_table;

# Remove the old table
drop table the_table_old;
```
