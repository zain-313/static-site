# static-site

# Main.go file

main () <br />  
"fs := http.FileServer(http.Dir("static"))" We use the FileServer function to create a handler which responds to all HTTP requests with the contents of a given FileSystem. 

For our FileSystem we're using the static directory relative to our application

"http.Handle("/", fs)" Next we use the Handle function to register our FileServer as the handler for all requests.

"http.ListenAndServe(":6060", nil)" We launch the server listening on port 6060.
