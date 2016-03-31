# Find which database has a table

```sql
set @tableName = 'table_name_here';

select  table_schema
from    information_schema.tables
where   table_name = @tableName;
```
