# ELK2
vim /etc/sysctl.conf
sysctl -w vm.max_map_count=262144
mkdir -p /opt/elk/elasticsearch/data
chmod g+rwx /opt/elk/elasticsearch/data
chgrp 0 /opt/elk/elasticsearch/dat
cd /opt/elk

docker compose up -d
