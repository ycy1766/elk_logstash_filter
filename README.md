# elk_logstash_filter
Custom logstash_filter for elk(elasticsearch,logstash,kibana)

## FileBeat configuration for Mysql SlowQuery

FileBeat configuration for Mysql SlowQuery parsing 

<pre>
    -
      paths:
        - {SlowQuery File Path}
      document_type: mysql-slow
      tail_files: false
      multiline:
        pattern: "^# Time:"
        negate: true
        match: after
</pre>

## FileBeat configuration for Mysql Errorlog

FileBeat configuration for Mysql Errorlog parsing

<pre>
    -
      paths:
        - {Mysql Error File Path}
      document_type: mysql_error
</pre>
