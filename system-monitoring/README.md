# System monitoring using telegraf and influxdb

1. Run the compose `docker-compose up -d`
2. Open [http://localhost:8086](http://localhost:8086) in the browser
3. Create a username and password, name your organization `tgm` and your first bucket `telegraf-bucket`
4. Choose quick start -> add data source -> Telegraf
5. Create a token and paste it in `telegraf/telegraf.conf`
6. Restart stack using `docker-compose up -d`
