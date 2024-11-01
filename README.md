LoggingMiddleware
What it Does
The LoggingMiddleware in this FastAPI application logs detailed information about each incoming HTTP request and its response. It records:

The HTTP method (e.g., GET, POST)
The request path (URL)
Request headers and body
The response status code
Processing time for each request
How to Use It
Define LoggingMiddleware in a separate file, such as middleware.py.
Add the middleware to your FastAPI app in the main application file:
python
复制代码
from middleware import LoggingMiddleware
app.add_middleware(LoggingMiddleware)
Example Log Output
When a request is made, the middleware generates logs like this:

yaml
复制代码
INFO: 2024-10-30 12:53:46
Request Method: GET
Request Path: /
Request Headers: {
  "host": "127.0.0.1:8000",
  "user-agent": "Mozilla/5.0 ...",
  ...
}
Request Body: No body
Response Status: 200
Response Time: 1.61ms
Benefits
This logging helps with:

Debugging: Understand request/response flows and identify issues.
Performance monitoring: Track response times and optimize as needed.
Insight into client requests: See request details, including headers and body content (when applicable).LoggingMiddleware
What it Does
The LoggingMiddleware in this FastAPI application logs detailed information about each incoming HTTP request and its response. It records:

The HTTP method (e.g., GET, POST)
The request path (URL)
Request headers and body
The response status code
Processing time for each request
How to Use It
Define LoggingMiddleware in a separate file, such as middleware.py.
Add the middleware to your FastAPI app in the main application file:
python
复制代码
from middleware import LoggingMiddleware
app.add_middleware(LoggingMiddleware)
Example Log Output
When a request is made, the middleware generates logs like this:

yaml
复制代码
INFO: 2024-10-30 12:53:46
Request Method: GET
Request Path: /
Request Headers: {
  "host": "127.0.0.1:8000",
  "user-agent": "Mozilla/5.0 ...",
  ...
}
Request Body: No body
Response Status: 200
Response Time: 1.61ms
Benefits
This logging helps with:

Debugging: Understand request/response flows and identify issues.
Performance monitoring: Track response times and optimize as needed.
Insight into client requests: See request details, including headers and body content.
