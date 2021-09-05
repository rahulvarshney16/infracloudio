docker pull infracloudio/csvserver:latest
docker pull prom/prometheus:v2.22.0
git clone https://github.com/infracloudio/csvserver.git
docker ps --format "{{.Names}}"
docker exec -it nostalgic_mirzakhani /bin/bash
netstat -tunlp | grep LISTEN
docker run -d -p 9393:9300 -e CSVSERVER_BORDER='Orange' -v /home/rahul/inputFile:/csvserver/inputdata infracloudio/csvserver:latest
curl -o ./part-1-output http://localhost:9393/raw

