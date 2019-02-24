# Authorization

- [ ] Insecure authorization design
- [ ] Only client side authorization
- [ ] Variable manipulation
- [ ] Direct access to resources
- [ ] IDOR


### IDOR explained - [OWASP](https://www.owasp.org/index.php/Testing_for_Insecure_Direct_Object_References_(OTG-AUTHZ-004))


### Compare request in Burpsuite - Look for different id's ...
Burpsuite Comparer - Compare request with 2 accounts
```
Proxy -> Intercept -> Click on(Intercept is off) -> Do the action -> Right-click on Send to comparer
```

### Write-ups
[reCAPTCHA bypass via HTTP Parameter Pollution](https://andresriancho.com/recaptcha-bypass-via-http-parameter-pollution/)

[Github SAML](http://www.economyofmechanism.com/github-saml.html)

[How I Could Steal Money from Instagram, Google and Microsoft](https://www.arneswinnen.net/2016/07/how-i-could-steal-money-from-instagram-google-and-microsoft/)

[Authentication bypass on Uber’s Single Sign-On via subdomain takeover](https://www.arneswinnen.net/2017/06/authentication-bypass-on-ubers-sso-via-subdomain-takeover/)

[Authentication bypass on Airbnb via OAuth tokens theft](https://www.arneswinnen.net/2017/06/authentication-bypass-on-airbnb-via-oauth-tokens-theft/)
