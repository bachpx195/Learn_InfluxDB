# Learn_InfluxDB

https://docs.influxdata.com/influxdb/v2.0/get-started/?t=Linux#start-influxdb

When installed as a service, InfluxDB stores data in the following locations:

. Time series data: /var/lib/influxdb/engine/
. Key-value data: /var/lib/influxdb/influxd.bolt.
. influx CLI configurations: ~/.influxdbv2/configs (see influx config for more information) .

To customize your InfluxDB configuration, use either command line flags (arguments), environment variables, or an InfluxDB configuration file. See InfluxDB configuration options for more information.



## Start InfluxDB

Start InfluxDB by running the influxd daemon:

> influxd


## Enable shell completion (Optional)
To install influx shell completion scripts, see influx completion.

InfluxDB “phone home”
By default, InfluxDB sends telemetry data back to InfluxData. The InfluxData telemetry page provides information about what data is collected and how it is used.

To opt-out of sending telemetry data back to InfluxData, include the --reporting-disabled flag when starting influxd.

> influxd --reporting-disabled
