# Clean Nexus3 release-repository

Groovy script to clean a release repository in nexus 3

## Setup

* In Nexus 3, go to "Server administration and configuration" -> "Manage scheduled tasks" -> "Create task"
* Select type "Execute script"
* Give a Name to task, select "Script language" as "Groovy" and select a "Task frequency" of your choice.
* Past the script "Cleanup.groovy" in "Script source"
* Click in "Create Task"

## Run

To run, you can click in "Run" button in the top of page.

## Logs

To see the logs of execution, in server side, you can:

    ```tail -f /usr/local/sonatype-work/nexus3/log/nexus.log ```

## Info

Tested in a Nexus Repository Manager version OSS 3.1.0-04

## License

This script is based in the following :

* https://github.com/danischroeter/nexus-repo-scripting/blob/master/src/main/groovy/deleteOldComps.groovy
* https://stackoverflow.com/questions/45589937/groovy-script-to-delete-artifacts-on-nexus-3-not-nexus-2
* https://raw.githubusercontent.com/xninjaxelitex/nexus3-cleanup-release-artifact/master/src/at/oebb/playground/Cleanup.groovy

