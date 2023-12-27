# Developing a Simple Webserver

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

HTML content creation is done

### Step 2:

Design of webserver workflow

### Step 3:

Implementation using Python code

### Step 4:

Serving the HTML pages.

### Step 5:

Testing the webserver

## PROGRAM:from http.server import HTTPServer,BaseHTTPRequestHandler
content="""
## WELCOME
"""
class HelloHandler(BaseHTTPRequestHandler): def do_GET (self): self.send_response (200) self.send_header('Content-type', 'text/html; charset=utf-8') Self.end_headers() self.wfile.write(content.encode())

server_address = ('', 80) httpd = HTTPServer (server_address, HelloHandler) httpd.serve_for

Type your code here


## OUTPUT:
![Screenshot 2023-12-27 202256](https://github.com/jokerjana/webserver/assets/147173630/3c5010b5-07ac-41d2-beb7-760b6687b451)


## RESULT:
The program is executed succesfully
