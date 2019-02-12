# ChatServer
This is the python chat server script that is run on our raspberry pi.  It allows users to send messages to all other devices
in the chat room.  To join the chat room, open a terminal window and type the following:

______________________________________________________________________________________

C:\python
>>>import socket
>>>s = socket.socket()
>>>s.connect(("10.0.1.10", 5000))

______________________________________________________________________________________

the command to send a message depends on if you are in python 2.7 or python 3.X:

python 2.7:    >>>s.sendall("Put your message here")

python 3.X:    >>>s.sendall(b"Put your message here")

to receive messages:    >>>s.recv(4048)
