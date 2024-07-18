start bin\windows\zookeeper-server-start.bat config\zookeeper.properties
start bin\windows\kafka-server-start.bat config\server.properties

Step 1: Go to the Downloads folder and select the downloaded Binary file.


Step 2: Extract the file and move the extracted folder to the directory where you wish to keep the files.

Step 3: Copy the path of the Kafka folder. Now go to config inside kafka folder and open zookeeper.properties file. Copy the path against the field dataDir and add /zookeeper-data to the path.

For example if the path is c:/kafka

Step 4: Now in the same folder config open server.properties and scroll down to log.dirs and paste the path. To the path add /kafka-logs

Step 5: This completes the configuration of zookeeper and kafka server. Now open command prompt and change the directory to the kafka folder. First start zookeeper using the command given below:

.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties


Step 6: Now open another command prompt and change the directory to the kafka folder. Run kafka server using the command:

.\bin\windows\kafka-server-start.bat .\config\server.properties

Now kafka is running and ready to stream data.
