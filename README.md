#### iOS-URI-Schemes-Abuse

A set of URI schemes bugs that lead Safari to crash/freeze. This shows URI schemes have weakness and can be used for nasty things. Apple is aware of the issue.

I decided to start looking at URI scheme after the crashsafari.com massacre. I wanted to find other ways to break Safari so here it is:

###### file-attack.html (file://)

This exploit will crash the user current tab without any specific requirement.

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/file-attack.html)

###### file-2-attack.html (file://)

This bug will crash the browser. The user must type the URI in the address bar and press enter.

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/file-2-attack.html)

###### mailto-iframe-attack.html (mailto://)

Freeze Safari and Safari/Firefox + Mail.app on OS X by sending a lot of datas to mailto: URI scheme.

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/mailto-iframe-attack.html)

###### sms-attack.html (sms://)

Freeze the SMS app by sending a lot of datas to sms: URI scheme. Require that the user either accept the popup / click on the link.

[Exploit](https://cdn.rawgit.com/pwnsdx/iOS-URI-Schemes-Abuse-PoC/master/sms-attack.html)
