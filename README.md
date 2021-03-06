# How Web Works Exercise

[Source](http://curric.rithmschool.com/springboard/exercises/how-web-works/ "Permalink to How Web Works Exercise")

## Part One: Solidify Terminology

In your own terms, define the following terms:

- What is HTTP?

  _A: HTTP stands for hypertext transfer protocol. It is a set of rules that govern how data is sent to or retrieved from a server._

- What is a URL?
  _A: This is often called a "web address," because it provides location information for a resource. URL stands for universal resource locator._

- Describe the different parts of a URL.

  _A: It contains information about the protocol, hostname, resource, and query. There is also a default port assigned if we don't specify one._

  - \_protocol:
  - _hostname: this is the human-readable name that the DNS server turns into an IP address_
  - _resource: specifies the content we're looking for on the site_
  - _query: this part is OPTIONAL and provides additional information like search terms, information from a form, etc._

- What is DNS?

  _A: DNS stands for Domain Name System. It works like an old school phone book for the **web** where the **hostname** we type into the address bar gets turned into an IP address that the computer can use. It can also do reverse lookups._

- What is a query string?

  _A: A query string is part of a URL and consists of key-value pairs that provide additional information to a get request. Example: typing a search term tells the computer exactly what part of the resource we're looking for. Or it might tell how we want data sorted._

- What are two HTTP verbs and how are they different?

  _A: GET and POST are two HTTP verbs. GET requests do not change server data; they are just requests to get information (a web page, search results). POST requests, on the other hand, do have side effects, such as updating a database (e.g., posting a message to social media)._

- What is an HTTP request?

  _A: An HTTP request is a request made by our browser according to the Hypertext Transfer Protocol. Using HTTP requests, we can retrieve information, such as html from Yahoo Finance. _

- What is an HTTP response?

  _A: An HTTP response is what comes back from the server when an HTTP request is sent._

- What is an HTTP header? Give a couple examples of request and response headers you have seen.
  _A: An HTTP header provides additional inforamtion about the request/response._

  - _Request header examples: Accept, Host, User-Agent, Accept-Language, Referer, Cache-Control_
  - _Response header examples: Connection, Date, Content-Type, Last-Modified, Cashe-Control_

- What are the processes that happen when you type “<http://somesite.com/some/page.html>” into a browser?

  _A:_
  _1. The browser sends the hostname to a DNS server to get the IP address (if the IP address is not already available in the local cache, router, or ISP)._
  _2. Then it makes a request to the server at the IP address to get the requested content. The request contains headers (re: the browser, preferred language, cookies, etc.)_
  _3. The server responds, usually with HTML, and a status code (which is 200 if successful)_
  \_4. The browser uses this information to build the DOM and make requests to get the other resources it needs, such as the images, CSS and JavaScript files, libraries, fonts, etc.

## Part Two: Practice Tools

1. Using curl, make a GET request to the _icanhazdadjoke.com_ API to find all jokes involving the word “pirate”

![Pirate jokes](pirate-jokes.png)

2. Use dig to find what the IP address is for _icanhazdadjoke.com_

_A: I typed 'dig icanhazdadjoke.com' into the terminal. There were three results, all with status code 300:_

- _104.27.178.209,_
- _104.27.179.209, and_
- _172.67.153.24_

3. Make a simple web page and serve it using python3 -m http.server. Visit the page in a browser.

_A: Here is the code I typed in:_
![Start a Python3 server](start-a-python3-server.png)
_Here is the rendered page at localhost:8000:_
![Rendered page on Python3 server](rendered-page-on-python3-server.png)

## Part Three: Explore Dev Tools

Build a very simple HTML form that uses the GET method (it can use the same page URL for the action) when the form is submitted.

See index.html:

![form with get method](form-with-get-method.png)

Add a field or two to the form and, after submitting it, explore in Chrome Developer tools how you can view the request and response headers.

![View request and response headers](view-request-response-headers-get.png)

Edit the page to change the form type to POST, refresh in the browser and re-submit. Do you still see the field in the query string?

_A: No_

Explore in Chrome how you can view the request and response headers, as well as the form data.

![View request and response headers and form data](view-request-response-headers-post.png)

## Part Four: Explore the URL API

At times, it’s useful for your JavaScript to look at the URL of the browser window and change how the script works depending on parts of that (particularly the query string).

[Read about the URL API](https://developer.mozilla.org/en-US/docs/Web/API/URL)

Try some of the code examples in the Chrome Console so that you can get comfortable with the basic methods and properties for instances of the URL class.

## Solution

You can [view our solution](http://curric.rithmschool.com/springboard/exercises/how-web-works/solution/index.html)
