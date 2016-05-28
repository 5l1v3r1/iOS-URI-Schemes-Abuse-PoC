#### iOS-URI-Schemes-Abuse-PoC

A set of URI schemes bugs that lead Safari to crash/freeze. This shows URI schemes have weakness and can be used for nasty things. Apple is aware of the issue.

I decided to start looking at URI schemes after the crashsafari.com massacre. I wanted to find other ways to break Safari so here it is:

###### file-attack.html (file://)

This bug will crash the user current tab without any specific requirement.

**Fixed in Safari Technology Preview 5**

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/file-attack.html)

###### file-2-attack.html (file://)

This bug will crash the browser on iOS and crash the current tab on OS X. **The user must type the URI in the address bar and press enter.**

**Fixed in Safari Technology Preview 5**

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/file-2-attack.html)

###### mailto-iframe-attack.html (mailto://)

This bug will freeze Safari and Safari/Firefox + Mail.app on OS X by sending a bunch of datas to mailto: URI scheme. **Only work if the user have at least one mailbox setup.**

**Not fixed yet**

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/mailto-iframe-attack.html)

###### sms-attack.html (sms://)

This bug will freeze the SMS app by sending a lot of datas to sms: URI scheme. **Require that the user either accept the popup or click on the link.**

**Not fixed yet**

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/sms-attack.html)
