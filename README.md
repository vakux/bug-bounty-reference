# Bug Bounty Reference

### Direct Object Reference (IDOR)
- [IDOR for X-Pid header allowed user with observer role to elevate privileges for SQS service of MCS (sqs.mcs.mail.ru) by using role from the different project.](https://hackerone.com/reports/1177451) by mrd0x1

### Unrestricted File Upload
- [Shell upload in http://widget.support.my.com/](https://hackerone.com/reports/317043) by danila
- [Unrestricted file upload on [ambassador.mail.ru]](https://hackerone.com/reports/854032) by organdonor

### Authentication Bypass
- [Improper Authentication - any user can login as other user with otp/logout & otp/login](https://hackerone.com/reports/921780) by korniltsev
- [Change any Uber user's password through /rt/users/passwordless-signup - Account Takeover (critical)](https://hackerone.com/reports/143717) by mongo
- [Account Takeover at worki.ru](https://hackerone.com/reports/725707) by r0hack
- [Forgot Password Page SMS Brute Force could lead to Account Takeover using Android/IOS app "About the house" via api.prodom.smart.space](https://hackerone.com/reports/944392) by jayesh25
- [Account takeover through password reset in cups.mail.ru](https://hackerone.com/reports/843160) by weev3kyaw
- [Lack of rate limitation on careers site allows the attacker to brute force the verification code](https://hackerone.com/reports/1075827) by iambouali
- [Full account takeover of any user through reset password](https://hackerone.com/reports/1175081) by saajanbhujel
- [Password reset link injection allows redirect to malicious URL](https://hackerone.com/reports/281575) by cablej 
- [Password Reset - query param overrides postdata](https://hackerone.com/reports/96636) by reecer

### Miscellaneous
- [Bypass Rate Limits on app.snapchat.com API Endpoint via X-Forwarded-For Header](https://hackerone.com/reports/727487) by sicarius
- [Client IP Spoofing using "X-Forwarded-For: 127.0.0.1" on "studio-app.snapchat.com" exposing bucket details](https://hackerone.com/reports/382678) by damian89
- [Error Page Content Spoofing or Text Injection](https://hackerone.com/reports/1245051) by princej_76


### recon win 
- [API on campus-vtc.com allows access to ~100 Uber users full names, email addresses and telephone numbers.](https://hackerone.com/reports/580268) by healdb
- [Administrator access to a Django Administration Panel on *.sc-corp.net via bruteforced credentials](https://hackerone.com/reports/128114) by shubs


host-header-injection
```
Host: example.com?.mavenlink.com
X-Forwarded-Host: evil.com
Referrer: https://evil.com
localhost.attacker.com or localhostattacker.com
Host: redacted.com?anythin<b>imran</b> or Host: redacted.com?"><a href='evil.com
```
