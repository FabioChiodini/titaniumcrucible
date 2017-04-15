# titaniumcrucible

Code in Python for an honeypot web site that logs to a remote logstash

The logstash configuration for this is similar to:

```
input {
  tcp {
    port => 5000
  }
}
```

