# Session Fixation

## Description
Session Fixation is an attack that permits an attacker to hijack a valid user session. The attack explores a limitation in the way the web application manages the session ID, more specifically the vulnerable web application. When authenticating a user, it doesn’t assign a new session ID, making it possible to use an existent session ID. The attack consists of obtaining a valid session ID (e.g. by connecting to the application), inducing a user to authenticate himself with that session ID, and then hijacking the user-validated session by the knowledge of the used session ID. The attacker has to provide a legitimate Web application session ID and try to make the victim’s browser use it.

## Prevention
* Ignore any session ID provided by the user's browser
* Always generate a new session to which the user will log in if successfully authenticated
* Sessions must be refreshed upon each login, logout and password reset event
