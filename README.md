# todoistPython

Script to get the number of todos for today and the filter "@focusHeute" from Todoist.
This script can be used standalone or as script for BetterTouchTool (https://folivora.ai)

## Configuration for BetterTouchTool

![Screenshot of MacOS Touchbar](todoistInBetterTouchTool.png)

1. Prerequesites
    1. Install python3
    1. In Todoist click your profile image and select integrations. At the bottom you will find the API-token.
1. Add new trigger
1. Select "Shell Script / Task Widget"
1. Set the following configuration options
    1. Execute script every ```300``` seconds (= every 5 minutes)
    1. Launch Path: ```usr/local/bin/python3```
    1. Parameters: ```-c```
    1. Environment Variables: ```TODOIST_API_TOKEN=```[Add your Todoist API-token here]
    1. Script: Insert the script focusHeuteAndToday.py or clone this repository and reference this file there.
