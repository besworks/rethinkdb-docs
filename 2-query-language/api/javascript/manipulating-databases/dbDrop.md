---
layout: api-command 
language: JavaScript
permalink: api/javascript/db_drop/
command: dbDrop
github_doc: https://github.com/rethinkdb/docs/edit/master/2-query-language/api/javascript/manipulating-databases/dbDrop.md
io:
    -   - r
        - object
related_commands:
    dbCreate: db_create/
    dbList: db_list/
    tableCreate: table_create/
---

{% apibody %}
r.dbDrop(dbName) → object
{% endapibody %}

Drop a database. The database, all its tables, and corresponding data will be deleted.

If successful, the operation returns the object `{dropped: 1}`. If the specified database
doesn't exist a `RqlRuntimeError` is thrown.

__Example:__ Drop a database named 'superheroes'.

```js
r.dbDrop('superheroes').run(conn, callback)
```
