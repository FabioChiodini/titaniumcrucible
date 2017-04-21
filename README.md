# titaniumcrucible

Code in Python for a very simple honeypot web site that sends logs to a remote logstash service.

## Dockerized version
In this repository you can also find the Dockerfile to run this application in Docker.

## Logstash input configuration
The most basic logstash input configuration for this is similar to:

```
input {
  tcp {
    port => 5000
  }
}
```

## Output

The log in kibana should show up like in this example log:

![Alt text](/images/tcLogELKwithgeoip.png "tcLogELKwithgeoip")

[This example log has been enhanced with a geoip filter implemented in logstash]
