# OSPREY-LTER-Harvest
Resources for the LTER metadata harvest

This config file tells OSPREY which projects and awards are linked to LTER data discoverable at DataONE.

# Adding a new LTER data pull #

1. Add the LTER data configuration to `config.json`
2. Pull the updates into OSPREY at /sites/all/modules/features/lter/OSPREY-LTER-Harvest
3. run `drush lter-recache-sites metadata {project-id}`
4. run `drush lter-clear-sparql-cache {project-id}`
5. run `drush lter-rdf-files`
6. login to the Virtuoso hosted on aws, run `./refresh-lter`
