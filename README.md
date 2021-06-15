* **sunucu.py** and **istemci.py** files must be run in Linux environments.
* Both files must be run with administrator rights.
## Server
* The server is listening on port 142 by providing the connection over TCP.
* The server sends the time in milliseconds and time information as "UTC+3" to the connecting clients.
* The server uses the time information of the operating system it is running on when setting the times of the connecting clients.
* The time zone can be changed to **"UTC+5"**, **"UTC-3"** via the **UTC** variable in **server.py**.
* Örnek olarak sunucunun işletim sisteminde zaman dilimi **"UTC+3"** ve sunucuda bulunan **UTC** değişkeni **"UTC+5"** olarak belirtilirse bağlanan istemcinin saati, sunucu saatinden 2 saat ileride olacak şekilde ayarlanacaktır.
## Client
* **istemci.py** çalıştırıldığında IP adresi olarak **sunucu.py**'nin IP adresi girilmelidir.
* Daha sonra sunucudan gelen milisaniye ve zaman bilgisi kullanılarak zaman bilgisi istenilen şekilde ayarlanır.
