# Auto_Index PostgreSQL Extension

## Overview

`auto_index` is a PostgreSQL extension that automatically identifies beneficial indexes during query execution and creates them dynamically using background workers.

## Files

| File                     | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `auto_index.c`           | Core implementation of planner/executor hooks, background worker logic, and index analysis. |
| `auto_index.h`           | Header file declaring functions, hooks, and required PostgreSQL includes.   |
| `auto_index.control`     | Extension control file with metadata for PostgreSQL.                        |
| `auto_index--1.0.sql`    | SQL script to set up the extension and required database objects.           |
| `Makefile`               | Build configuration for compiling the extension with PGXS.                  |

### Build and Install

```bash
make
sudo make install
