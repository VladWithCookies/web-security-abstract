# CSRF

## Description
Cross-Site Request Forgery (CSRF) is a type of attack that occurs when a malicious web site, email, blog, instant message, or program causes a user's web 
browser to perform an unwanted action on a trusted site when the user is authenticated. A CSRF attack works because browser requests automatically include 
all cookies including session cookies. Therefore, if the user is authenticated to the site, the site cannot distinguish between legitimate requests and forged requests.

## Prevention
- [ ] Properly setup CORS
- [ ] Include server generated CSRF token to all forms and check it on every request
- [ ] Always use `SameSite` cookie attribute for session cookies
- [ ] Do not use GET requests for state changing operations
- [ ] Use custom request header (browsers do not allow JavaScript to make cross origin requests with custom headers) 
- [ ] Double Submit Cookie (send a random value in cookies and inside request params and verify values match on the server) or use cookie with \__Host prefix for cookie that contains CSRF token. 
