#### iOS-URI-Schemes-Abuse

A set of URI schemes bugs that lead to crash/freeze of the Safari browser. This shows URI schemes have weakness and can be used for nasty things. Apple is aware of the issue.

###### file-attack.html (file://)

This exploit will crash the user current tab without any specific requirement.

###### file-2-attack.html (file://)

This bug will crash the browser. The user must type the URI in the address bar and press enter.

###### mailto-attack.html (mailto://)

Freeze Safari and Safari + Mail.app on OS X by sending a lot of datas to mailto: URI scheme.

###### sms-attack.html (sms://)

Same as mailto-attack, may work less better than mailto-attack.
