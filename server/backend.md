# Backend

## About

**Node.js** is an [open-source](https://en.wikipedia.org/wiki/Open-source_software), [cross-platform](https://en.wikipedia.org/wiki/Cross-platform) [JavaScript](https://en.wikipedia.org/wiki/JavaScript) [run-time environment](https://en.wikipedia.org/wiki/Runtime_system) that executes JavaScript code outside of a browser. JavaScript is used primarily for [client-side scripting](https://en.wikipedia.org/wiki/Client-side_scripting), in which scripts written in JavaScript are embedded in a webpage's HTML and run client-side by a JavaScript engine in the user's web browser. Node.js lets developers use JavaScript to write command line tools and for [server-side scripting](https://en.wikipedia.org/wiki/Server-side_scripting)—running scripts server-side to produce [dynamic web page](https://en.wikipedia.org/wiki/Dynamic_web_page) content before the page is sent to the user's web browser. Consequently, Node.js represents a "JavaScript everywhere" paradigm,[\[7\]](https://en.wikipedia.org/wiki/Node.js#cite_note-7) unifying [web application](https://en.wikipedia.org/wiki/Web_application) development around a single programming language, rather than different languages for server side and client side scripts.



## Installation

```text
Git clone https://github.com/escape-room-samk/backend.git
cd backend
npm install
npm start
```

## Mongoose Database 

* MongoDB **stores data in flexible, JSON-like documents**, meaning fields can vary from document to document and data structure can be changed over timeThe document model **maps to the objects in your application code**, making data easy to work with
* **Ad hoc queries, indexing, and real time aggregation** provide powerful ways to access and analyze your data
* MongoDB is a **distributed database at its core**, so high availability, horizontal scaling, and geographic distribution are built in and easy to use
* MongoDB is **free and open-source**. Versions released prior to October 16, 2018 are published under the AGPL. All versions released after October 16, 2018, including patch fixes for prior versions, are published under the [Server Side Public](https://www.mongodb.com/licensing/server-side-public-license)
* 
### Run Mongoose 

```text
Mongod
```

## API

{% api-method method="post" host="https://172.17.2.10" path="/api/qrReader" %}
{% api-method-summary %}
QR Reader
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="Boolean" type="boolean" required=false %}
True or False
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" required=false %}
the value
{% endapi-method-parameter %}

{% api-method-parameter name="devID" type="string" required=false %}
ID of the Device
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{ error: false, message: "Data added" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{ error: true, message: "Error adding data" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}





{% api-method method="post" host="https://172.17.2.10" path="/api/motionsensor" %}
{% api-method-summary %}
Motion Sensor
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="value" type="string" required=false %}
the value
{% endapi-method-parameter %}

{% api-method-parameter name="devID" type="string" required=false %}
ID of the Device
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{ error: false, message: "Data added" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{ error: true, message: "Error adding data" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="post" host="https://172.17.2.10" path="/api/rfidReader" %}
{% api-method-summary %}
RFID Sensor
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="value" type="string" required=false %}
the value
{% endapi-method-parameter %}

{% api-method-parameter name="devID" type="string" required=false %}
ID of the Device
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{ error: false, message: "Data added" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{ error: true, message: "Error adding data" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



{% api-method method="post" host="https://172.17.2.10" path="/api/imageReader" %}
{% api-method-summary %}
Image Detecotor
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="Boolean" type="boolean" required=false %}
True or false
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" required=false %}
the value
{% endapi-method-parameter %}

{% api-method-parameter name="devID" type="string" required=false %}
ID of the Device
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{ error: false, message: "Data added" }
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{ error: true, message: "Error adding data" }
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}





