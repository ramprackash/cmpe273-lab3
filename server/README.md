Distributed Cache Server
========================

$ mvn clean package

# How to run servers forever
$ nohup ./bin/run_server_A.sh 0<&- &> /tmp/app-a.log &
$ nohup ./bin/run_server_B.sh 0<&- &> /tmp/app-b.log &
$ nohup ./bin/run_server_C.sh 0<&- &> /tmp/app-c.log &

# Or using the convenient script
$ ./run_server.sh

# Cache Server endpoints: 
Server_A => http://localhost:3000/cache/
Server_B => http://localhost:3001/cache/
Server_C => http://localhost:3002/cache/


