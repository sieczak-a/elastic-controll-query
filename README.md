# elastic-controll-query
Elasticsearch project which enables controlling queries used by users

On elasticsearch instance need to be enabled module called "slowlog"
https://www.elastic.co/guide/en/elasticsearch/reference/current/index-modules-slowlog.html

for example in file log4j2.properties
set:
logger.index_search_slowlog_rolling.name = index.search.slowlog
logger.index_search_slowlog_rolling.level = trace
logger.index_search_slowlog_rolling.appenderRef.index_search_slowlog_rolling.ref = index_search_slowlog_rolling
logger.index_search_slowlog_rolling.additivity = false
