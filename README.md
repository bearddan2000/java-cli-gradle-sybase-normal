# java-cli-gradel-sybase-normal

## Description
Creates a small database table
called `dog` and populates it
with a single row. This table, `dog`, has been normalized to 3NF. All output normally
seen in a terminal will be in `java-srv/log` which will dump to the screen. The project may seem to hang but the logs from the container must be written to the project this can take up to 3 min.

## Tech stack
- docker-wait
- java
- gradel
  - log4j
  - sybase driver

## Docker stack
- gradle:jdk11
- datagrip/sybase

## To run
`sudo ./install.sh -u`
Creates java-srv/log

## To stop
`sudo ./install.sh -d`
Removes java-srv/log

## For help
`sudo ./install.sh -h`

## Credit
- [Sybase driver and connection example](https://razorsql.com/docs/help_sybase.html)
