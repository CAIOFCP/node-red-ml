FROM nodered/node-red-docker:latest
# installing an editor

USER root
RUN mkdir /home/root
RUN apt-get update && apt-get -y install  python-pip nano
RUN find /usr/lib/python2.7 -type d -exec chmod 755 {} \;
RUN find /usr/lib/python2.7/*.py -exec chmod 644 {} \;
RUN pip install tensorflow keras 
RUN npm install node-red-dashboard node-red-contrib-python3-function 

