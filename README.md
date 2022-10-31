# sso-and-translation-layer-db-monitor
Record all manual database updates/changes for SSO and Translation Layer projects

## Branch Naming Convention
We are using a specific naming convention for branches in Github to provide consistency across developers and projects that execute manual queries outside of code repositories.

> Branch names will include the following data elements separated by a hyphen “-” symbol:

* Story Type (i.e. Insert/Update/Delete)

* Database

* Developer Initials

* Jira Ticket Number

Example:

**{ Insert/Update } / { SSO/TL } - { Developer Initials } - { Jira Ticket # }**

> Update/sso-lr-ktlo-12345

## File Naming Convention
We are using a specific naming convention for files in Github to provide consistency across developers and projects that execute manual queries outside of code repositories.

> File names will include the following data elements separated by a underscore “_” symbol:

* Story Type (i.e. insert/update/delete)

* Database

* Developer Initials

* Date (mm_dd_yyyy format)

Example:

**{ insert/update } / { sso/tl } _ { Developer Initials } _ { Date }**

> update_sso_lr_10_31_2022.js

> rollback_sso_lr_10_31_2022.js

## Process

1. Create a new branch following the naming convention described above

2. Add the script file that contains the database actions into src directory

3. Select the js/ or sql/ directory depending on the query language

4. Add the script file that contains the rollback plan into the ../rollback/ directory 

5. Commit and push the changes

6. Create a PR and follow the workflow process
