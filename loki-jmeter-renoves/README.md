## USAGE

docker build . -t myjmeter

docker run -e "TARGET_HOSTNAME=158.177.221.40" -e "TARGET_PORT=30372" -e "LOADC=" myjmeter

LOADC Default:
const(7,20s) line(7,7,20s) line(7,8,20s) const(9,20s) line(9,9,20s) const(10,20s) const(10,20s) const(10,20s) line(10,10,20s) const(9,20s) line(9,9,20s) line(9,8,20s) line(8,7,20s) line(7,6,20s) line(6,5,20s) const(4,20s) line(4,4,20s) line(4,3,20s) line(3,2,20s) const(1,20s) const(1,20s) const(1,20s) const(1,20s) line(1,1,20s) line(1,3,20s) const(5,20s) const(5,20s) line(5,5,20s) line(5,7,20s) line(7,6,20s) const(5,20s) line(5,5,20s) const(6,20s) const(6,20s) line(6,6,20s) const(7,20s)
