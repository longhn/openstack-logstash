
The files in this repo help use [logstash](http://logstash.net/) to aggregate and process OpenStack logs. 

In the example below, `agent.conf` is copied to `/etc/logstash` and `patterns` dir is copied to `/etc/logstash`.
You must include the default [grok-patterns](https://github.com/logstash/logstash/blob/master/patterns/grok-patterns)
in the same directory. Here is an example to start logstash with these patterns on each OpenStack node.

-using with elastisearch and kibana
  java -jar logstash-1.3.3-flatjar.jar agent -f elasticsearch.conf -- web

-using with statsd
