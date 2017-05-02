Use kurento-docker for KMS, see : https://github.com/Kurento/kurento-docker

Add MongoDB + nodeJS front project.

run :

docker run -d --name kurento -p 8888:8888 -p 8433:8433 -p 0:65535/udp -p 8443:8443 -p 27017:27017 -it edwinnss/webrtc-docker

8888 & 8433 > kurento-media-server
8443 > nodeJS project
27017 > MongoDB
65535 > KMS turn server
