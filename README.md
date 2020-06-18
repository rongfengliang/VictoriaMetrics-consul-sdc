# test vmagent with consul sdc
* consul

```code
curl -X PUT -d '{"id": "prometheus-app","name": "prometheus-app","address": "prometheus","port": 9090,"tags": ["appname:demo","appversion:v1"],"checks": [{"http": "http://prometheus:9090/metrics", "interval": "5s"}]}'  http://127.0.0.1:8500/v1/agent/service/register
```

