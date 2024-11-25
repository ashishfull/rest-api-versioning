# REST API Versioning

This repository demonstrates multiple approaches to versioning REST APIs using **Spring Boot**. API versioning is crucial for maintaining backward compatibility while allowing new features or changes.

## Table of Contents
- [Overview](#overview)
- [Techniques Demonstrated](#techniques-demonstrated)
- [How to Run](#how-to-run)
- [API Endpoints](#api-endpoints)
- [Example Responses](#example-responses)
- [License](#license)

---

## Overview

This project showcases the following REST API versioning techniques:
- URI Versioning
- Request Parameter Versioning
- Header Versioning
- Media Type (Content Negotiation) Versioning

Each version returns a simple response representing a person's name.

The core API versioning logic is implemented in the [Controller Path](https://github.com/ashishfull/rest-api-versioning/blob/main/src/main/java/com/ashishrai/rest_api_versioning/controller/PersonController.java)

---

## Techniques Demonstrated

1. **URI Versioning**  
   Example: `/v1/person`, `/v2/person`

2. **Request Parameter Versioning**  
   Example: `/person?version=1`, `/person?version=2`

3. **Header Versioning**  
   Example:  `GET /person/header Header: X-API-VERSION=1`

4. **Media Type Versioning (Content Negotiation)**  
Example:  `GET /person/header Header: Accept: application/vnd.company.app-v1+json`


---

## How to Run

1. Clone the repository:
`bash
git clone https://github.com/username/rest-api-versioning.git
cd rest-api-versioning`
2. Build and run the project using Maven:
`mvn spring-boot:run`
3. Access the APIs using a REST client like Postman, Talend or curl.



