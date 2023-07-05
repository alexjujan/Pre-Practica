# Pre-Practica

This project’s purpose is to collect data from  a sensor(temperature, humidity and pressure) and send them through the MQTT Broker to Grafana for data visualization.

Steps I followed to complete this project:
1.	I started to research the technologies that I needed to use. 

•	First thing first, I installed and got familiar with the Waspmote PRO IDE tool, which is a software development kit used for writing and uploading code and it can also be used to monitor the serial output and for debugging.
	Download link: https://development.libelium.com/waspmote-ide-v06/download-ide-windows


•	Research about MQTT(Message Queuing Telemetry Transport) Broker technology:
	MQTT is a publish/subscribe, extremely simple and lightweight messaging protocol, designed for constrained devices and low-bandwidth, high-latency or unreliable networks, where battery power is critical.
	The broker is a key agent in MQTT protocol. The broker is a server which receives all the frames and distributes each one of them to the subscribers clients.
	Configuration, the user can set:
	IP Address: Server IP address.
	Port number: Server port number.
	User: Server user name to log in the MQTT system.
	Password: Server password to log in the MQTT server.
	Topic template: Topic of your message.
	Message template: Data structure of your message.


•	Research about Node-Red program:
	Installing Node-Red, which is a flow-based programming tool and we are using it for data processing.
	Download link: https://nodejs.org/en
	Steps for running the program after downloading:
	Open Command Prompt 
	Write this command “node --version && npm –version”. The output should be something like this: v18.15.0 / 9.5.0.
	Write this command “npm install -g --unsafe-perm node-red”. The installation will start. After the installation is done write this command “node-red” and the program should start.


•	Introduced Grafana:
	Grafana is a multi-platform open source analytics and interactive visualization web application. It provides charts, graphs, and alerts for the web when connected to supported data sources.
	Logged in with the given username and password: user: interviu.practica pass: beiapractica.
	As a preview it should take you here:


•	From what I researched until now I understood that:
	In order to transfer data to the Internet, I need to connect to a Meshlium device which is an IoT gateway that connects the Libelium Plug & Sense device to the internet. 
	After completing these steps, the data transmitted is sent to the BEIA broker from which I will gather the information that I want to visualize in Grafana. 


2.	From here on I started to write the code in Waspmote PRO IDE which you can find here on github 
