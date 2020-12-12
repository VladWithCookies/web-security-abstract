# Header Injection

## Description
The ability to manipulate an application's response by setting the HTTP Host header to arbitrary values.

## Prevention
* Ensure all incoming HTTP headers are properly sanitized to prevent malicious header values from being included in the response or backend business logic.
