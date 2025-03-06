# Changelog for ocenv

Changlog starts with changes after version 2024-08-23.

## 2025-03-06

- Rename "pull_ocenv_main" to "update_ocenv"
- Automatically distribute updated ocenv to other RAC nodes when calling
  update_ocenv
- Add "update_autoupgrade" method
  - This will try to download the current autoupgrade.jar from oracle.com
  - Only if the current ORACLE_HOME contains /rdbms/admin directory
  - If possible it will replace file in /rdbms/admin with the downloaded file
- Add alias for "oratop" (part of RDBMS ORACLE_HOME)
- Fix most of help-texts to <80 column width
- Add check for current Bash version (script does not work in Bash 2.x)
  - Testing is only done in Bash 4.x, script will show a WARNING for Bash 3.x
- Do not use v$instance for prompt in login.sql

## 2024-11-29

- Enhance handling of PDBs in pdbsql
- add "get_sqlzauberkasten_oracle" method to download SQL-Zauberkasten
  - This will be downloaded and extracted to SCRIPT_DIR/sql/zauberkasten
  - include "zauberkasten/sql" directory in SQLPATH
- Prevent alias for "ls" and "which" to be used by script-commands
