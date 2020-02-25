FROM bimgbily/hadoop:latest

CMD until hdfs dfs -mkdir -p /apps/tez/ && hdfs dfs -put $TEZ_ARCHIVE_NAME /apps/tez/tez.tar.gz; do echo ... && sleep 1; done && schematool -dbType postgres -initSchema && hiveserver2