#  Command Injection

## Description
This ability to execute operating system commands by injecting shell metacharacters ( ; & | ) into an application's runtime environment is known as a Command Injection 
or shell injection vulnerability.

## Prevention
- [ ] Avoid passing user-controllable input in functions or system calls that interface with the operating system environment or invoke third-party applications
- [ ] Validate the input against a whitelist of permitted values
- [ ] Validate the input length
- [ ] Validate that the input contains only alphanumeric values, ignoring all other escape characters or whitespace string

