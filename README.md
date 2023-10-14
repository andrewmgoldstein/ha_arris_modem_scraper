# ha_arris_modem_scraper
Scraper to fetch arris modem status and publish to mqtt

This is based work in https://github.com/mmiller7/Arris_modem_scrape/

This has been tested on my Arris TM1602AP2 firmware TS0901103BE_091417_1602.TM

This script should allow you to scrape the modem status data and write it out to a MQTT broker where you can then use something like HomeAssistant to take actions based on the data (graph it, issue automations to cycle a smartplug, etc)


Files:
arris_modem_signal_dump.sh - the script scrapes/parses the data publishing JSON to MQTT
arris_modem_signgal.yaml - initial YAML to run the script periodically and import the startup status

