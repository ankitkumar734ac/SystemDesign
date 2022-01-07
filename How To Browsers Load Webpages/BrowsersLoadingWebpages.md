Browsers loading webpages
HTTP stands for HyperText Transfer Protocol.

- It is, like the name suggests, a set of rules for querying the web.
- It works on a client-server model, where the client, in most cases, the browser, makes a network request, and waits for the server to respond.

Browsers use HTTP requests to fetch us web pages.

- When we enter a website URL, the browser creates an HTTP request for the HTML of the page, on our behalf, and sends it to the server on which the website is hosted.
- The HTTP response from the server is read by the browser and rendered for us beautifully as web pages instead of the raw HTML returned.


Q. If the URL is only referring to an HTML file request, how does the Browser know what all other resources (CSS, JS) the web page needs?

Ans:- The HTML file will have the resource dependencies listed down. Browser parses the HTML file and figures out the next set of requests it needs to make.

For example, here’s a super simplified HTML snippet
`
<!DOCTYPE html>
<html lang="en">
<head>
    <link rel="stylesheet" href="styles.css">
    <title>Learning By Doing!</title>
</head>
<body>
    <h1>Learn By Doing</h1>
    <img src="img.jpg">
    <script src="script.js"></script>
</body>
</html>
`
This HTML page will tell the Browser to make 3 additional HTTP requests for
- style.css
- img.jpg
- script.js


----------------------------------------------------------------
These properties calls out some important information regarding the request-response process for a request

- Request URL → URL of the resource fetched (what you typed in the Browser’s URL bar)
- Request Method → Action to be done. “GET” is for downloading (getting) some resource
- (Response) Status Code → How the server responded to the request
- - “200 OK” means a successful request
- - As this is a successful “GET” request, server will have sent some data back i.e, website’s HTML content
- Remote Address → Address of the application serving the resource requested. Has two sections
- - IP address → Location of the server hosting the resource (eg: 163.53.78.128)
- - Port → Location of the application within the server, serving the resource (eg: 443)

This was the URL we used to visit the Flipkart page - https://www.flipkart.com/

The first part of the URL denotes the protocol to use for communication with the server at www.flipkart.com.

- https is a more secure version of the HTTP protocol and is very widely used instead of http
- HTTPS servers can be accessed at Port 443 by default

Response headers contain more information about the HTTP response sent by the server.

- Content-Type → Type of the response content (eg: text/html → HTML)
- Server → Web server software used by the server (eg: nginx, Apache, AmazonS3)
Similarly, the Request headers contain more information about the HTTP request sent to the server

Note:-

<a herf="https://app.netlify.com/drop">Link </a>
On to deployment
Follow the steps given to deploy your “Top 4” page and get a shareable link for it

TODO

- Open https://app.netlify.com/drop 
- Drag and drop the folder with your index.html, styles.css files to “Drag and drop” section of this page (section with the white background on the right)
- Netlify will generate a shareable link to your web page now (Note: Refresh the page and repeat Step 2, if you get an error here)
- Visit the link and verify your page is being displayed correctly
















