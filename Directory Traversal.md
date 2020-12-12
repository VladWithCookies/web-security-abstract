# Directory Traversal

## Description
The ability to get an application to resolve file paths and to display the file’s content. 
It allows the attacker to access and explore the server’s file system, possibly extracting sensitive information.

## Prevention
* Avoid passing user-supplied input to filesystem APIs
* Perform strict input validation against parameters that are intended to be used for file system operations. These include path validation and absolute path checking of user-supplied data
