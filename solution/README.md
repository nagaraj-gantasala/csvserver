--part I--
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

 i need to check to wright shall script about  10 such entries in current directory to generate any number of entries.

--partII--
created docker-compose.yml
and run docker-compose up -d

-- i am not able to run the container with this basic and smaple  yml  

--part III--
partIII

docker pull prom/prometheus:v2.22.0

docker images 
docker run -p 9393:9393 prom/prometheus	.
note : instend  od infracloud/csv server image i am run conatiner with prem/premotheus image with post 9090
instend prometheus.yml tomorrow we can use our own docker-compose.yml for application monotoring in permotheus.

Thank you.
