## File-Transfer-Server-using-Socket

In this program we will see how to use python to transfer files over network using sockets.
Python is very helpful as it has modules for every single thing you want to do.

# Python program for client side
In client side I have created one server socket and connect it to  same port and IP of server. I have used 127.0.0.1 loopback address to use both client and server on same machine. Take file name from user which is to be downloaded from sever. If file is available at server it will send to client. So here open file with ‘wb’  i.e. write binary and save it to client side

@client.py

# Python program for server side
In server side I have created one server socket and bind it to  same port as in client program. Then we have used listen(max_client) method to take server online. After that I have called accept() method in while loop. The for loop is used to scan every file on server side and find file requested by client. Method os.listdir(dir_name) returns the array of file names in given directory. If file found the open() it and read() it to send to client. Read it part by part and send it to client.

@server.py

To run this code, run server.py in one terminal and client.py on another terminal. Enter file name at client side and download file from server

