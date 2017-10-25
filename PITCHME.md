![](https://disrupt-and-innovate.org/wp-content/uploads/2015/09/burning-platform.jpg)
---

## Platform testing?

* API testing
* E2E testing
* Regression testing

+++

## Understand what should be tested

* Webservice: API - used to exchange data between applications
* has an interface - WSDL
* operates over HTTP
* protocol - SOAP, REST

---

## Testing an API

* Software to send calls, get output, log response
* Log timing
* Error handling

---

## What to Test For?

* Ordinary conditions, obvious
* Typical conditions
* Stressing the System, Limits and Tolerance
* Badly-formed data, real-time input, not expected types, handling exceptions

+++

## Tests

* Check the results of the action
* Describe the test results and unexpected events
* Smoke, Sanity, CRUD, Negative, Boundary, Security

+++

## Structure

![](https://i.imgur.com/YRNcvwU.png)

---

## Security testing

* Request, Response, Message formats
* Authorization/Authentication, SSL

---

## Security testing

Surface detection

![](https://blog.smartbear.com/wp-content/uploads/2014/11/HackYourAPI3-600x351.jpg)


---

## Security testing

* Metadata
* Discovery
* Brute Force

---

## Security testing

* Fuzzing - generating randomized data
* Sending unexpected invalid input
* Malicious input
* SQL Injection

---

## SQL Injection


```
petstore.com/api/v1/pet/123

queries:
SELECT * FROM pets WHERE petID='” + petId +”‘”;
```

---

## SQL Injection

```
petstore.com/api/v1/pet/’%20or%20’1’=’1

queries:
SELECT * FROM pets WHERE petID = ‘’ or ‘1’ = ‘1’

```

---

## Tools

* cURL
* Postman
* Charles
* mitmproxy
* Lithium
* JMeter

