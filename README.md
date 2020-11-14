Implemening web access including redirect.
A web client to access a webpage on a web server
If the server redirects the request to another URL using status code 301 or 302, then client program should access the new URL. 
Repeat the process till status code received is 200 or 403 or 404. Save the content of the received file in your local directory as per path given in the redirected
URL and also note down the Last-Modified header for this file. Next time this URL is invoked, client should send the headers If-Modified-Since and it should process
the response accordingly. 

Invoke program as

./filename.py -url <URL>
