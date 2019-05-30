# Ax Change

> ISV solution for Dynamics 365 for Finance and Operations products for simplifying the integration process with third-party web-services

## What it is

`AxChange` is a universal solution for configuring integration processes with third-party web services.
Unlike the traditional integration tools of the `Dynamics 365 for Finance and Operations` system with third-party products, AxChange does not require modifications by developers. This is a new approach to integrating products `Dynamics 365`, where the initiator of integration is the system itself, and not another service.
To start using it, just get the solution and configure the mapping structure and request to send to a third-party service.

See the [Quick start](quickstart.md) guide for more details.

## Features

- Supports HTTP / HTTPS protocols
- Create your own dynamic structures related to Entity
- Creating requests
    - With different methods: GET | POST | PUT | PATCH | DELETE
    - With different content types: form-data | text | form-urlencoded | binary
- Support for importing data received in response
    - With Data management
    - By writing using standard Entity
- Support for request authorization
    - Basic
    - Bearer
    - Using cookie
    - Based on data from another request
- Creating actions for received response
    - Import data
    - Sending a new request
- Adding headers manually to the request
- Use of certificates
- Maintaining the history of requests and response
- Logging of internal processes
