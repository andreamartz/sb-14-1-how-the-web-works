# How Web Works Exercise

[Source](http://curric.rithmschool.com/springboard/exercises/how-web-works/ "Permalink to How Web Works Exercise")

## Part One: Solidify Terminology

In your own terms, define the following terms:

- What is HTTP?

  A: HTTP stands for hypertext transfer protocol.

- What is a URL?
  A: THis is often called a "web address." URL stands for universal resource locator.

- Describe the different parts of a URL.

  _A: It contains information about the protocol, hostname, resource, and query. THere is also a default port assigned if we don't specify one._

  - _hostname:_
  - _resource: what content we're looking for_
  - _query: this part is OPTIONAL and provides additional information like search terms, information from a form, etc._

- What is an IP?

  _A: IP stands for Internet Protocol._

- What is DNS?

  _A: DNS stands for Domain Name System. It works like an old school phone book for the **web** where the **hostname** we type into the address bar gets turned into an IP address that the computer can use. It can also do reverse lookups._

- What is a query string?
- What are two HTTP verbs and how are they different?

  _A: GET and POST are two HTTP verbs. POST requests_

- What is an HTTP request?
- What is an HTTP response?
- What is an HTTP header? Give a couple examples of request and response headers you have seen.
- What are the processes that happen when you type “<http://somesite.com/some/page.html>” into a browser?

## Part Two: Practice Tools

1. Using curl, make a GET request to the _icanhazdadjoke.com_ API to find all jokes involving the word “pirate”
2. Use dig to find what the IP address is for _icanhazdadjoke.com_
3. Make a simple web page and serve it using python3 -m http.server. Visit the page in a browser.

## Part Three: Explore Dev Tools

Build a very simple HTML form that uses the GET method (it can use the same page URL for the action) when the form is submitted.

Add a field or two to the form and, after submitting it, explore in Chrome Developer tools how you can view the request and response headers.

Edit the page to change the form type to POST, refresh in the browser and re-submit. Do you still see the field in the query string? Explore in Chrome how you can view the request and response headers, as well as the form data.

## Part Four: Explore the URL API

At times, it’s useful for your JavaScript to look at the URL of the browser window and change how the script works depending on parts of that (particularly the query string).

[Read about the URL API](https://developer.mozilla.org/en-US/docs/Web/API/URL)

Try some of the code examples in the Chrome Console so that you can get comfortable with the basic methods and properties for instances of the URL class.

## Solution

You can [view our solution](http://curric.rithmschool.com/springboard/exercises/how-web-works/solution/index.html)
