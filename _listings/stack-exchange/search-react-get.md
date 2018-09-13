---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 0
info:
  title: Stack Exchange Search Subscription
  description: This is a subscription template for Stack Exchange search.
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
/search:
  get:
    summary: Search for React
    description: Search questions with React in the title.
    operationId: search
    x-api-path-slug: search-get
    parameters:
    - in: query
      name: intitle
      default: React
    - in: query
      name: order
      default: desc
    - in: query
      name: site
      default: stackoverflow
    - in: query
      name: sort
      default: activity
    responses:
      200:
        description: OK
    tags:
    - Search
---
