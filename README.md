# Introduction
This repository contains files related to the Open API Specification (OAS) defined by Swagger.

# Known issues
This section lists some current known issues we experience related to the OAS

## AWS API Gateway
When trying to upload the openapi.yml to AWS API Gateway we get the below error and warnings, even if the file is valid according to SwaggerHub.

```
Your API was not imported due to errors in the Swagger file.

    Unable to create resource at path '/registrations/{email}/{eventId}': A sibling ({id}) of this resource already has a variable path part -- only one is allowed
    Additionally, these warnings were found:
    More than one server provided. Ignoring all but the first for defining endpoint configuration
    Unsupported model type 'StringSchema' in 201 response to method 'POST /events'. Ignoring.
    Unsupported model type 'StringSchema' in 404 response to method 'POST /events'. Ignoring.
    Unsupported model type 'StringSchema' in 201 response to method 'POST /registrations'. Ignoring.
    Unsupported model type 'StringSchema' in 400 response to method 'POST /registrations'. Ignoring.
    Unsupported model type 'StringSchema' in 409 response to method 'POST /registrations'. Ignoring. 
```
