# HTTP protocol

## What is it?
An application layer protocol that governs how data is transmitted between clients (usually web browsers) and servers.

---

## Key components

### Client-Server Model
HTTP follows the client-server model, where clients (e.g., web browsers) send requests to servers, and servers respond with the requested resources (e.g., web pages, images, data).

### Stateless Protocol
HTTP is stateless. Each request from the client to the server is treated as an independent transaction without any knowledge of previous requests.

### Request Methods
- GET: Requests data from the server.
- POST: Submits data to be processed by the server (e.g., form submissions).
- PUT: Uploads data to the server, replacing the current resource.
- DELETE: Requests the server to delete the specified resource.

### Uniform Resource Identifiers(URIs)
URIs are used to identify resources on the web. They provide a unique address that clients can use to access resources on the server.

---

## HTTP Headers
HTTP headers are additional pieces of information sent by both the client and the server in the HTTP request and response messages. These headers provide metadata and instructions about the request or response, helping to control the behavior of the communication. Some common headers include:

- User-Agent: Identifies the client application or browser making the request.
- Accept: Specifies the media types (e.g., HTML, JSON, XML) that the client can handle in the response.
- Content-Type: Specifies the media type of the data being sent in the request or response body.
- Authorization: Used to send credentials (e.g., username and password) for authentication purposes.
- Cache-Control: Instructs caching behavior for both the client and server.

---

## HTTP Parameters
HTTP parameters are key-value pairs that are added to the URL as part of an HTTP request. They are used to pass additional data to the server or to specify certain options for the request. Parameters are typically used with the GET method, where they are appended to the URL after a question mark (?) and separated by ampersands (&). For example:

`https://example.com/search?query=apple&type=fruit`

In this example, the `query` and `type` parameters are passed to the server, and the server can use them to perform a search and respond with relevant results.

---

## HTTP status codes
- Informational (1xx)
- Successful (2xx)
- Redirection (3xx)
- Client error (4xx)
- Server error (5xx)

### Common status codes
- 200 OK: The request was successful, and the server has returned the requested data.
- 201 Created: The request was successful, and a new resource was created as a result.
- 204 No Content: The server successfully processed the request, but there is no data to return (e.g., after a successful DELETE request).
- 301 Moved Permanently: The requested resource has moved to a new URL permanently, and the client should update its references accordingly.
- 400 Bad Request: The server could not understand the request due to a client error, such as malformed syntax.
- 404 Not Found: The requested resource could not be found on the server.
- 500 Internal Server Error: A generic error message indicating that the server has encountered a problem and cannot fulfill the request.
