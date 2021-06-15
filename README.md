* **server.py** and **client.py** files must be run in Linux environments.
* Both files must be run with administrator rights.
## Server
* The server is listening on port 142 by providing the connection over TCP.
* The server sends the time in milliseconds and time information as "UTC+3" to the connecting clients.
* The server uses the time information of the operating system it is running on when setting the times of the connecting clients.
* The time zone can be changed to **"UTC+5"**, **"UTC-3"** via the **UTC** variable in **server.py**.
* For example, if the time zone is specified as "UTC+3" in the server's operating system and the UTC variable on the server is "UTC+5", the time of the connecting client will be set to be 2 hours after the server time.
## Client
* When **client.py** is run, the IP address of **server.py** should be entered as the IP address.
* Then, the time information is adjusted as desired by using the millisecond and time information from the server.
