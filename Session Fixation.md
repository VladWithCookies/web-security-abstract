# Session Fixation

## Description


## Prevention
* Ignore any session ID provided by the user's browser
* Always generate a new session to which the user will log in if successfully authenticated
* Sessions must be refreshed upon each login, logout and password reset event
