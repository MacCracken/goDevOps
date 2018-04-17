# Section 2 Notes

## Requests

HTTP Requests in GO

* The Go standard library includes the HTTP package which is used for sending and recieving requests
* You can create a client instance or make a sinple requests with a default client

## HTTP Headers

* Headers are used to provide metadata about HTTP requests
* usage in this repo/course use headers primarly for authentication credentials

## REST API Content

* REST API requests and responses typically have JSON formated content
* Go includes JSON support for marshaling and unmarshaling this content

## Error Handling

* REST APIs have typical error responses as any HTTP request might have
* Often with REST APIs there will be additional error information included in the body of the response

### Assement Questions

Q1. What is the simplest way to make a GET request?
A1. a. Use the http package Get() function

Q2. What header is used to identify the client application?
A2. c. The User-Agent header

Q3. What header is used to identify the payload type of a POST request?
A3. Content-Type

Q4. What is the typical content type of a REST request payload?
A4. d. JSON

Q5. What are the functions used for converting JSON data to a Go structure and vice versa?
A5. a. json.Marshalandjson.Unmarshal

Q6. What class of HTTP status codes are used for client errors?
A6. c. 400’s

Q7. What class of HTTP status codes are used for server errors?
A7. d. 500's