# Authentication
- [ ] Password strength enforcement
- [ ] Authentication bypass
- [ ] Unauthenticated URL access
- [ ] Password brute force
- [ ] Default account(admin)
- [ ] Reset password link


### Password strength enforcement
```Register a new account and use a easy password```


### Password brute force 
Bruteforce with Burpsuite or use [https://github.com/vanhauser-thc/thc-hydra] also works on different protocols 
```Proxy -> Intercept -> Click on(Intercept is off) -> Do the action -> Right-click on Send to Intruder -> Click on Intruder and do your stuff!```


### Reset password link
Create 2 accounts
```Proxy -> Intercept -> Click on(Intercept is off) -> Click on reset password on the website -> Action(Send to comparer) -> Compare the results in the compare tab look for id's and hashes```


### Resources 
[OWASP](https://www.owasp.org/index.php/Top_10-2017_A2-Broken_Authentication)


### Write-ups
[E-mail me your password](http://blog.jr0ch17.com/2018/Please-email-me-your-password/)

[Bypass Captcha](https://medium.com/@know.0nix/bypassing-captcha-like-a-boss-d0edcc3a1c1)

[How I was able to compromise any user account](https://medium.com/@logicbomb_1/bugbounty-how-i-was-able-to-compromise-any-user-account-via-reset-password-functionality-a11bb5f863b3)
