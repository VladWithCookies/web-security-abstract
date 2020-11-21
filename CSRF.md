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
- [ ] Double Submit Cookie (send a random value in cookies and inside request params and verify values match on the server*)

\* To enhance the security of this solution include the token in an encrypted cookie - other than the authentication cookie (since they are often shared within subdomains) - and 
then at the server side match it (after decrypting the encrypted cookie) with the token in hidden form field or parameter/header for AJAX calls. This works because a sub domain 
has no way to over-write an properly crafted encrypted cookie without the necessary information such as encryption key.
