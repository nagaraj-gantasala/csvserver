docker pull infracloudio/csvserver:latest
docker pull prom/prometheus:v2.22.0
git clone https://github.com/infracloudio/csvserver.git
docker run -it infracloudio/csvserver:latest
error inputdata file not available or directory
inputFile created in my current location
docker run -d -v /root/csvserve/soulation/inputFile:csvserver/inputdata infracloudio/csvserver
docker run -d -p 9393:9300 -v /root/csvserve/soulation/inputFile:csvserver/inputdata infracloudio/csvserver
open port and able to see output(http://ip172-18-0-39-cd7u04m3tccg00c8k8bg-9393.direct.labs.play-with-docker.com/)
docker run -d -p 9393:9300 -e CSVSERVER=BRODER='Orange' -v /root/csvserve/soulation/inputFile:csvserver/inputdata infracloudio/csvserver
