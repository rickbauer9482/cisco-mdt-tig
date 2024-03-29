Create at Telegraf, InfluxDB, and Grafana (TIG) stack using docker-compose

Copy the repo to the folder where you want to run docker-compose from and modify the docker-compose.yml and telegraf.conf files for your needs. Local volumes for the containers will be created in the working directory where you run the "docker-compose up -d" command.

Example: Docker-Tig is my working directory

Docker-TIG/docker-compose.yml

Docker-TIG/telgraph.conf

Docker-TIG/telegraf-volume/

Docker-TIG/telegraf/

Docker-TIG/influx-volume/

Docker-TIG/grafana-volume/

Docker-TIG/vols

You must configure the data source in Grafana with the information you used in your telegraf.conf file.

Now, you are ready to receive telemetry data from your Cisco routers and switches. Add your IP Address to the Telemetery sample configuration file and cut and paste to your switches.

Subsequently, you can run "docker-compose stop" and "docker-compose start" to stop and start your new containers.

This link from Cisco DEVNET should get you started with the Telemetry subscriptions on your IOS-XE devices.

https://developer.cisco.com/docs/ios-xe/#!streaming-telemetry-quick-start-guide/enabling-streaming-telemetry

