# Find which stored procedure contains text

```sql
set @text = '%text here%';

select  *
from    information_schema.routines
where   routine_definition like @text
order by routine_name;
```
