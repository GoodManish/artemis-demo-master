
myLaptop MINGW64 ~/Desktop/apache-artemis-2.28.0/bin
- $ ./artemis create myTestBroker --user=admin --password=password
Creating ActiveMQ Artemis instance at: C:\Users\vanma\Desktop\apache-artemis-2.28.0\bin\myTestBroker

--allow-anonymous | --require-login:
Allow anonymous access?, valid values are Y, N, True, False
Y

Auto tuning journal ...
done! Your system can make 1.84 writes per millisecond, your journal-buffer-timeout will be 544000

You can now start the broker by executing:

   "C:\Users\vanma\Desktop\apache-artemis-2.28.0\bin\myTestBroker\bin\artemis" run

Or you can setup the broker as Windows service and run it in the background:

   "C:\Users\vanma\Desktop\apache-artemis-2.28.0\bin\myTestBroker\bin\artemis-service.exe" install
   "C:\Users\vanma\Desktop\apache-artemis-2.28.0\bin\myTestBroker\bin\artemis-service.exe" start

   To stop the windows service:
      "C:\Users\vanma\Desktop\apache-artemis-2.28.0\bin\myTestBroker\bin\artemis-service.exe" stop

   To uninstall the windows service
      "C:\Users\vanma\Desktop\apache-artemis-2.28.0\bin\myTestBroker\bin\artemis-service.exe" uninstall

myLaptop MINGW64 ~/Desktop/apache-artemis-2.28.0/bin
- $ cd myTestBroker/bin/

myLaptop MINGW64 ~/Desktop/apache-artemis-2.28.0/bin/myTestBroker/bin
$ ls
artemis.cmd  artemis-service.exe*  artemis-service.exe.config  artemis-service.xml

myLaptop MINGW64 ~/Desktop/apache-artemis-2.28.0/bin/myTestBroker/bin
- $ ./artemis-service.exe install
2023-03-21 13:15:54,465 INFO  - Installing the service with id 'artemis-myTestBroker-0.0.0.0'

myLaptop MINGW64 ~/Desktop/apache-artemis-2.28.0/bin/myTestBroker/bin
- $ ./artemis-service.exe status
Stopped

myLaptop MINGW64 ~/Desktop/apache-artemis-2.28.0/bin/myTestBroker/bin
- $ ./artemis-service.exe start
2023-03-21 13:16:05,544 INFO  - Starting the service with id 'artemis-myTestBroker-0.0.0.0'

- -------------------Check broker.xml if port bind error comes.. change PORT like below  eg. 5673 instead of 5672
  <!-- AMQP Acceptor.  Listens on default AMQP port for AMQP traffic.-->
         <acceptor name="amqp">tcp://0.0.0.0:5673




# artemis-demo
Dispatcher and Receiver example over Artemis MQ using Java Spring Boot

# YouTube

Watch the tutorial on YouTube

[![Watch the tutorial on YouTube](https://img.youtube.com/vi/2FVXUvrtBr4/maxresdefault.jpg)](https://youtu.be/2FVXUvrtBr4)

[![Watch the tutorial on YouTube](https://img.youtube.com/vi/_PM4II2LBr0/maxresdefault.jpg)](https://youtu.be/_PM4II2LBr0)
