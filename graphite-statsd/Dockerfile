FROM hopsoft/graphite-statsd:latest
LABEL org.freenas.version="false"                       \
      org.freenas.version="1"                             \
      org.freenas.web-ui-protocol="http"                \
      org.freenas.expose-ports-at-host="true"           \
      org.freenas.web-ui-port="5080"                      \
      org.freenas.autostart="true" \
      org.freenas.bridged="true" \
      org.freenas.dhcp="false" \
      org.freenas.address="192.168.0.50" \
      org.freenas.hostname="PigLet" \
      org.freenas.port-mappings="5080:80/tcp,2003:2003/tcp,2004:2004/tcp,2023:2023/tcp,2024:2024/tcp,8125:8125/tcp,8126:8126/tcp"                                       \
      org.freenas.volumes="[                            \
          {                                             \
              \"name\": \"/opt/graphite/conf\",         \
              \"descr\": \"graphite config\"            \
          },                                            \
          {                                             \
              \"name\": \"/opt/graphite/storage\",      \
              \"descr\": \"graphite stats storage\"     \
          },                                            \
          {                                             \
              \"name\": \"/etc/nginx\",                 \
              \"descr\": \"nginx config\"               \
          },                                            \
          {                                             \
              \"name\": \"/opt/statsd\",                \
              \"descr\": \"statsd config\"              \
          },                                            \
          {                                             \
              \"name\": \"/etc/logrotate.d\",           \
              \"descr\": \"logrotate config\"           \
          },                                            \
      ]"
      org.freenas.static-volumes="[					\
          {								\
              \"container_path\": \"/host/tank/Graphit1/log\",				\
              \"host_path\": \"/var/log\",				\
              \"readonly\": \"false\"					\
          }								\
      ]" 
