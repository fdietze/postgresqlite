# PostgreSQLite

Use postgres like sqlite.

# Example Usage

```bash
$ postgresqlite test-db "create table numbers(id serial primary key, number real not null)"
create table numbers(id serial primary key, number real not null)
CREATE TABLE

$ postgresqlite test-db "insert into numbers (number) values (5)"
insert into numbers (number) values (5)
INSERT 0 1

$ postgresqlite test-db "select * from numbers"
select * from numbers
 id | number 
----+--------
  1 |      5
(1 row)

$ du -sh test-db
40M	test-db
```



# Install

Requires: `docker`.

Add the postgresqlite script to your path.

```bash
# for example
PATH=$PATH:$HOME/projects/postgresqlite
```


