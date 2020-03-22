FROM java:8

WORKDIR /usr/src/app

ENV LOADC="line(10,40,180s) line(40,20,180s) line(20,30,180s) line(30,10,180s)" THROTTLE=100


CMD sed -i "s/TARGET_HOSTNAME/$TARGET_HOSTNAME/g" local/appOps-shaping.config && sed -i "s/TARGET_PORT/$TARGET_PORT/g" local/appOps-shaping.config && echo "TARGET: $TARGET_HOSTNAME $TARGET_PORT" && bin/jmeter -n -t local/the_thing.jmx -l local/results.jtl -q local/appOps-shaping.config -J throttle="$THROTTLE" -J load_profile="$LOADC"

COPY . .
RUN chmod -R 777 /usr/src/app