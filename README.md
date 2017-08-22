# elk_logstash_filter
Custom logstash_filter for elk(elasticsearch,logstash,kibana)

## FileBeat configuration for Mysql SlowQuery

<pre>
    -
      paths:
        - {SlowQuery File Path)
      document_type: mysql-slow
      tail_files: false
      multiline:
        pattern: "^# Time:"
        negate: true
        match: after
</pre>
