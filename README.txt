User Instructions
=================

Developer Push Down List
========================
Date: 2009-08-15
  Subject: search_files_directories.module needs to handle overlapping directory trees when indexing
  Subject: search_files_directories.module needs to handle duplicate directory entries on Add/Edit
  Subject: search_files.module needs to handle duplicate helper entries on Add/Edit
  Subject: we need some url/path rewriting
  Subject: replace SQL LIMIT clause by db_query_range() for non-MySQL compatibility

Date: 2009-08-14
  Subject: Titles and Descriptions should no longer be wrapped in t(), see http://drupal.org/node/140311
  Subject: node MIME type vs. search_files EXTENSION file classification

Date: 2009-07-26
  Subject: name space cleanup
    This module is almost name space clean, including function names, database
    tables and columns or identifiers in foreign database tables. However, the
    "search" module put a dirty little length limit in the `type` column of the
    {search_dataset} table. Same for {search_index} table. As soon as the
    lenght limit disappears, change the identifiers:
    - search_files_dir
    - search_files_att
    + search_files_directories
    + search_files_attachments

