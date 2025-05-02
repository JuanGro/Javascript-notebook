# How Do Webpages Work?

Understanding how webpages load helps demystify what happens when you visit a website. Here's a detailed, step-by-step breakdown of the process.

## 1. User Requests a Webpage

When a user types a URL into the browser (e.g., `https://example.com`), the browser breaks it down:

- `https` — protocol
- `example.com` — domain
- (optional) `/page` — specific path to a resource

The browser extracts the **domain name** to initiate a request.

```plaintext
URL: https://example.com
Protocol: HTTPS
Domain: example.com
```

## 2. DNS Lookup

The browser queries a **DNS (Domain Name System)** server to resolve the domain to an IP address.

```plaintext
example.com ➝ 93.184.216.34
```

This IP address identifies the server where the website is hosted.

## 3. Browser Sends an HTTP(S) Request

Using the resolved IP, the browser sends an **HTTP/HTTPS request** to ask for the website content:

```http
GET / HTTP/1.1
Host: example.com
```

The server receives this request and prepares a response.

## 4. Server Responds

The server replies with essential webpage files:

- `index.html` — the main HTML document
- CSS files — for styling
- JavaScript files — for interactivity
- Images, fonts, etc.

```http
HTTP/1.1 200 OK
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head><title>Example</title></head>
  <body><h1>Hello, World!</h1></body>
</html>
```

## 5. Browser Renders the Page

The browser builds and displays the page:

1. **Parses HTML** to create the **DOM (Document Object Model)**.
2. **Applies CSS** to style the DOM elements.
3. **Executes JavaScript** to enable interactivity.
4. **Displays** the final rendered page to the user.

```html
<!-- index.html -->
<h1 style="color:blue">Welcome!</h1>
<script>
  alert('Page Loaded!');
</script>
```

## 6. Ongoing Communication (Optional)

Modern webpages often continue communicating with the server using:

- **AJAX**: Send/receive data without refreshing.
- **WebSockets**: Maintain an open connection for real-time updates.

```javascript
// Example: AJAX call using Fetch API
fetch('/api/data')
  .then(response => response.json())
  .then(data => console.log(data));
```

## Summary

From URL to rendered page, the journey includes:

- DNS resolution
- HTTP(S) request/response
- HTML parsing & DOM creation
- CSS & JS execution
- Optional asynchronous communication

This process allows webpages to be fast, interactive, and dynamic.
