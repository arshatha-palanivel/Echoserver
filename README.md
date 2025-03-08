# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
```
Client:
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'ARSHATHA P, 212222230012,06-03-2025')
    print(f'Received: {s.recv(1024)!r}')

Server:
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_server((HOST, PORT)) as s:
    conn, addr = s.accept()
    with conn:
        print(f'Connected by {addr}')
        while data := conn.recv(1024):
            conn.sendall(data)
```
## OUTPUT:

![00000000000](https://github.com/user-attachments/assets/cbd25671-26ed-4b45-afbf-4ddaf3cdd82e)


## RESULT:
The program is executed successfully
