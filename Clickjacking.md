# Clickjacking

## Description
Clickjacking is technique whereby a webpage is loaded via an `iframe` and subsequently covered with deceptive content to trick a user into 
invoking an action on the underlying webpage is known as a Clickjacking attack.

## Prevention
- [ ] Include `X-Frame-Options` or `Content-Security-Policy` header
- [ ] Prevent session cookies from being included when the page is loaded in a frame using the `SameSite` cookie attribute
- [ ] Implementing JavaScript code in the page to attempt to prevent it being loaded in a frame
