# titaniumcrucible

Code in Python for an honeypot web site that logs to a remote logstash service.


The most basic logstash input configuration for this is similar to:

```
input {
  tcp {
    port => 5000
  }
}
```


The log in kibana should show up like in this example log:


[This example log has been enhanced with a geoip filter implemented in logstash]
