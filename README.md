# TriggerTest
## What this does
The purpose of this repository is to test the release-trigger element of the github workflow.

## What is release-trigger
Is a simple piece of code which can be configured to send a webhook event to a defined webserver (currently a test URL stored as a github secret).
Through comments, you can select the triggering activity (such as new releases, commits, PRs etc).

## What happens after triggering
This script collects info regarding all of the commits from the past release, all of the info coming from dependabot and such which will be stored in a specific .json file, and create a .json file to send as payload of the POST request (the webserver will then start all of the AI architecture).


Developed in the context of the 25/26 Polito x Hitachi challenge.
