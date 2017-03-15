# pivotal-tc-server

This image is based on https://hub.docker.com/r/clotech/tcserver/~/dockerfile/

## How to run

I'm currently not able to run the image directly.  But I can do this:

docker run -it --rm -p 8080:8080 -p 8443:8443 -p 6969:6969 rbosse/pivotal-tc-server /bin/bash

/web/tcserver/01/bin/tcruntime-ctl.sh status

/web/tcserver/01/bin/tcruntime-ctl.sh start 

After this, you should be able to view these urls:

http://192.168.99.100:8080/ returns home page of tc server
and
http://192.168.99.100:8080/manager returns the tomcat manager
