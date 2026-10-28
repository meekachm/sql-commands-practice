# SQL Commands Practice

A small coursework / practice exercise using **SQLite** to explore a one-to-many relationship between albums and songs.

## What's included

[`songs_albums.sql`](songs_albums.sql) contains:

- `Albums` and `Songs` table definitions, including a foreign-key declaration.
- Sample albums and songs.
- Queries that list the data and join songs to their albums.
- Filters using `BETWEEN` and `LIKE`.

The original assignment prompts are preserved as comments alongside the SQL.

## Run locally

With the SQLite command-line tool installed, clone this repository, enter its directory, and run:

```bash
sqlite3 :memory: < songs_albums.sql
```

This uses a temporary in-memory database, so each run starts clean. The script includes SQLite CLI formatting commands (`.headers` and `.mode`); those lines are not portable SQL for other database clients.

## Expected examples

- The date-range query selects albums published from 1970 through 1980.
- The joined date-range query returns songs from those albums.
- The album-name filter matches `Hotel California`.

## Scope

This is a focused SQL learning exercise, not a complete application. It demonstrates table creation, sample data, joins, and filtering. It does not include an automated test suite.

## Original reference

The original README also linked to this [SQL Fiddle](http://sqlfiddle.com/#!7/a34037/2). Its current availability has not been verified.

