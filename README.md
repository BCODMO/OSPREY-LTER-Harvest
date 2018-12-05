# OSPREY-LTER-Harvest
Resources for the LTER metadata harvest

This config file tells OSPREY which projects and awards are linked to LTER data discoverable at DataONE.

# Adding a new LTER data pull #

1. Add the LTER data configuration to config.json
2. Pull the updates into OSPREY at /sites/all/modules/features/lter/OSPREY-LTER-Harvest
3. run the LTER reloader script at /scripts/lter-triplestore-load.sh
4. A cronjob on the Triplestore server checks for updated LTER data every 20min on the hour
