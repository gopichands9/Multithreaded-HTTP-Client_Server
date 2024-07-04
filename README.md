# Multithreaded-HTTP-Client_Server

<h4>Port Number Used: 9090 </h4>

<h4>Running the Server: </h4>

1.	Open cmd from the Server folder where the file HttpServer.java is located. </br>
2.	Run the command “javac HttpServer.java” – This will compile the java file </br>
3.	Run the command by passing the port number “java HttpServer.java 9090” – This will java program and start our server. </br>
4.	Congratulations, our server is ready to accept the incoming requests from client. </br>

<h4>Running the Client: </h4>
1.	Open cmd from the Client folder where the file HttpClient.java is located.</br>
2.	Run the command “javac HttpClient.java” – This will compile our java file.</br>
3.	Run the HttpClient by passing the hostname, port number, HttpMethod, path using the command “java HttpClient localhost 9090 get </br>./server_to_client.html” – This will fetch a file named “server_to_client.html” from server and sends it back to client with code 200 OK.</br>
4.	Run the above command with invalid file using the command “java HttpClient localhost 9090 get ./server_to.html” – This will return “404 file not found”.</br>
5.	Run the above command by changing httpmethod & path using the command “java HttpClient localhost 9090 put ./client_to_server.html” – this will perform the put operation.</br>
       
<h4>Shutdown of server using termination signal:</h4>
1.	Open cmd from the Client folder where the file HttpClient.java is located.</br>
2.	Run the command “javac HttpClient.java” – This will compile our java file.</br>
3.	Run the HttpClient by passing the hostname, port number, HttpMethod, path using the command “java HttpClient localhost 9090 over ./” – This will close all the open sockets in server and shutdown the server.</br>
4.	Run any command related to GET or PUT, It will say “Connection refused”.</br>
Ex: “java HttpClient localhost 9090 get ./client_to_server.html”</br>

