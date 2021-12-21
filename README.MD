Create at Telegraf, InfluxDB, and Grafana (TIG) stack using docker-compose

Simply copy the repo the folder where you want to run docker-compose from, modify the docker-compose.ylm and telegraf.conf files for your needs. Local volumes for the contailers will be created in the working directory where you run the "docker-compose up -d" commnad.

Example: Docker-Tig is my working directory

Docker-Tig/docker-compose.yml

Docker-Tig/telgraph.conf

Docker-Tig/grafana-volume

Docker-Tig/influx-volume

You will have to configure the data souce in Grafana with the information you used in your telegraf.conf file.

Now you ready to receive telemetry data from your Cisco routers and switches. Add your IP Address to the Telemetery sample configuration file and cut and paste to you switches.

Subsequentially, you can run "docker-compose stop" and "docker-compose start" to stop and start your new containers.

This link from Cisco DEVNET should get you started with the Telemetry subscriptions on your IOS-XE devices.

https://developer.cisco.com/docs/ios-xe/#!streaming-telemetry-quick-start-guide/enabling-streaming-telemetry

