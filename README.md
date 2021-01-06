# thread pooled http server

Use CURL to issue a DELETE request:

curl -i -X "DELETE" http://localhost:8080/myfile.html

To test this operation use CURL to issue a PUT request to upload a file:

curl -i --upload-file localfile.html -X PUT http://localhost:8080/serverfile.html

Use CURL to issue a POST request that URL-encodes its data values like an HTML form (on one line):

curl -i --data-urlencode 'Name=Gareth Wylie' --data-urlencode 'Age=24' --data-urlencode 'Formula=a + b' -X POST http://localhost:8080/registration

Use CURL to issue a POST request that includes a "Profile-pic" field whose value is a PNG file of the user:

curl -i --form "Name=Gareth Wylie" --form "Age=24" --form "Profile-pic=@/Users/gareth/gareth.png" -X POST http://localhost:8080/registration

Use CURL to issue a POST request that formats its data values like an HTML form (on one line):

curl -i --data 'Name=Gareth Wylie' --data 'Age=24' --data 'Formula=a + b' -H 'Content-Type:text/plain' -X POST http://localhost:8080/registration

Use CURL to issue a GET request, in this case to list the server's root content directory:

curl -i http://localhost:8080/




