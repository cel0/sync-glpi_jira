# Synchronize GLPI and JIRA using Python APIs

These python scripts can be used to synchronize GLPI tickets with JIRA issues.

### Features ###
* Sync new tickets
* Sync Status
* Sync comments

### Python APIs used: ###

* A python interface to the GLPI webservices plugin: https://github.com/mcphargus/python-glpi

* JIRA Python Library: https://github.com/pycontribs/jira

# Setup #

### GLPI Webservices Configuration ###

1) Log in to GLPI

2) Setup -> Webservices -> Click in Add

3) Fill fields and select options:
* Name: sync-glpi_jira
* Child entities: Yes
* Enabled services: Yes
* Compression enabled: No
* Log connections: Logs
* Debug: No
* SQL pattern for services: .*
* IPv4 address range: server-ip_sync-glpi_jira - server-ip_sync-glpi_jira
* Other fields: null

4) Save

### JIRA API Configuration ###

1) Log in to GLPI

2) System

3) Change "Accept remote API calls":	OFF to ON

4) Update
