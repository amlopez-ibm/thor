FROM java:8

WORKDIR /usr/src/app


CMD  bin/jmeter -n -t local/ttr.jmx -l local/results.jtl -q local/appOps-shaping.config 

COPY . .
COPY local/openshift-origin-client-tools-v3.11.0-0cbc58b-linux-64bit/oc /usr/local/bin/oc
RUN chmod -R 777 /usr/src/app