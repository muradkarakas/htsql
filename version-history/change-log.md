---
description: Be sure to not miss out on new features and improvements!
---

# Change Log

## 2020-04-30 \(Version 0.0.4\)

### Bug fixes

* Page expire time calculation was wrong. It is fixed.
* Postgresql Demo was not working due to database row identifying strategy. It is replaced with new one \(see Improvements for deail\).

### Improvements

* Demo database objects are created in SODIUM\_DEMO user in Oracle Container database \(with using "alter session set "\_ORACLE\_SCRIPT"=true;" command\). After this modification, demo database user names for both Oracle and Postgresql are same. 
* Pseudo columns 

  * `oid` in Postgresql database
  * `rowid` in Oracle database

  are not used anymore. Developer must set [key-column-name](../language-reference/tags/data-block/#key-column-name-property) property if he/she want to have a writable datablock.

## 2020-04-29 \(Version 0.0.3\)

### Improvements

\`\`[`key-column-name`](../language-reference/tags/data-block/#key-column-name-property)property added to the [data block tag](../language-reference/tags/data-block/)

## 2020-04-28 \(Version 0.0.2\)

### Bug fixes

While parsing string literals in sqlx files, &lt; and &gt; characters are not copied into string. Sqlx file lexer fixed.

## 2020-04-23 \(Version 0.0.1\)

### Improvements

From now on, pNotify is used as client library for message function. An also, a new variant has been added to message function.
