# OPITZ CONSULTING Oracle scripts

## Description

This library contains scripts created and used by consultants from OPITZ CONSULTING Deutschland GmbH. They help us when working on our customers servers which are not allways configured in a homogenous way.

In general these scripts should be licensed GPL-3.0 or later

## Scripts

### ocenv

| License          | OS compatibility | Required Shell |
| ---------------- | ---------------- | -------------- |
| GPL-3.0 or later | Linux, AIX       | Bash >= 4.0    |

This script should be used by sourcing it directly or via .bashrc. It will create an alias "ocenv" in the .bashrc of the current user when sourced

After sourcing the script, the commands envhelp and varhelp can be used to get more information about available commands and variables respectively.
