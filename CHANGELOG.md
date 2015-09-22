# Changelog

## 0.6.4    UNRELEASED

* ...


## 0.6.3    2015-08-20

* Deparsing
  * COUNT(*) [@JackDanger](https://github.com/JackDanger)
  * Window clauses [Chris Martin](https://github.com/cmrtn)
  * CREATE TABLE/VIEW/FUNCTION [@JackDanger](https://github.com/JackDanger)
* Return exact location for parser errors [@JackDanger](https://github.com/JackDanger)


## 0.6.2    2015-08-06

* Speed up gem install by not generating rdoc/ri for the Postgres source


## 0.6.1    2015-08-06

* Deparsing: Support WITH clauses in INSERT/UPDATE/DELETE [@JackDanger](https://github.com/JackDanger)
* Make sure gemspec includes all necessary files


## 0.6.0    2015-08-05

* Deparsing (experimental)
  * Turns parse trees into SQL again
  * New truncate method to smartly truncate based on less important query parts
  * Thanks to [@mme](https://github.com/mme) & [@JackDanger](https://github.com/JackDanger) for their contributions
* Restructure extension C code
* Add table/filter columns support for CTEs
* Extract views as tables from CREATE/REFRESH VIEW
* Refactor code using generic treewalker
* fingerprint: Normalize IN lists
* param_refs: Fix length attribute in result


## 0.5.0    2015-03-26

* Query fingerprinting
* Filter columns (aka columns referenced in a query's WHERE clause)
* Parameter references: Returns all $1/$2/etc like references in the query with their location
* Remove dependency on active_support


## 0.4.1    2014-12-18

* Fix compilation of C extension
* Fix gemspec


## 0.4.0    2014-12-18

* Speed up build time by only building necessary objects
* PostgreSQL 9.4 parser


See git commit log for previous releases.
