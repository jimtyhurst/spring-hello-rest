# spring-hello-rest

Trivial RESTful service responds to /greeting request with a JSON response.

This project gives me a simple service that I can deploy to a cloud server, in order to test a cloud service.

## Usage

Simplest request is:

    http://localhost:8080/greeting

which leads to default JSON response:

    { "id": 1,
      "content": "Hello, World!"
    }

'name' property can be provided:

    http://localhost:8080/greeting?name=Chris

to customize the response string:

    { "id": 2,
      "content": "Hello, Chris!"
    }

The value of "id" is based on a counter that increments on each request.