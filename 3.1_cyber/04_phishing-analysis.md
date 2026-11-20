# Phishing Investigation

## Task 1 --- Analyse a Suspicious Email

>**Subject**: ⚠ Urgent: Your Account Will Be Locked in 24 Hours!
>
>**From**: Security Team <support@secure-verification-update.com>
>
>**To**: you@example.com
>
>Hello User,
>
>We detected unusual activity on your account. For your security, your access will be temporarily suspended within 24 hours unless you verify your information.
>
>Please click the link below to avoid interruption:
>
>👉 Verify Your Account Now
[http://secure-update-verification.com/login-confirmation](https://secure-update.verify-account-check.example.com/login/redirect/authentication_step2/?sessionid=3f9a2b8c7d1e44aa92f1b0f8f&token=invalid123456789&continue=http%3A%2F%2Fupdate-alert-confirmation.example.net%2Fverify%2Fuser%2Fsecurity%2Fcheck%2F?id=889201&source=email_warning)
>
>Failure to verify may result in permanent loss of access and data.
If you believe this is a mistake, reply with your full name, date of birth, and password so we can assist you.
>
>**Thank you,**
>
>**Account Support Team**
>
>**Security Department**



### Questions

Who appears to be the sender?
“Security Team” support@secure-verification-update.com. The name is generic and no real organisation is named. The domain is built from trust words (secure, verification, update) to look official.
Does the email create urgency or pressure?
Yes. “Urgent”, “Locked in 24 Hours”, and a threat of “permanent loss of access and data” push the reader to act without thinking.
Are there spelling or grammar mistakes?
Almost none, but there are other red flags: the generic greeting “Hello User”, a vague signature, and a request to reply with full name, date of birth and password. No legitimate company asks for a password by email.
Does the link match the organisation domain?
No. The sender domain, the displayed link and the real URL are three different domains, and the URL also redirects to a fourth (update-alert-confirmation.example.net).

### Reflection

Explain why attackers use phishing emails.

------------------------------------------------------------------------

## Task 2 --- Link Inspection

Hover over the link in the email (or copy link) and inspect the URL.

### Screenshot

(Add screenshot)

### Questions

1.  Does the displayed link match the actual URL? No. The displayed text is http://secure-update-verification.com/login-confirmation, but the real destination is secure-update.verify-account-check.example.com/....
2.  Are there unusual domain names? Yes: multiple different domains, long hyphenated names with words like “secure” and “verify”, misleading subdomains (the real domain is example.com), unencrypted http://, and a suspicious tail with sessionid, token and a continue= redirect.

### Reflection

Displayed link text can hide the real destination, which may be a fake login page or a malware download. Checking takes seconds, while a single click can cost you your account. Instead of clicking, go to the official site by typing its address yourself.
