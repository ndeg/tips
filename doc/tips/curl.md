# Curl

## Test sending a mail with a SMTP server

Given that `yoursmtpserver` is listening on standard port 25 and a text file `body-email` exists :

```bash
curl smtp://yoursmtpserver --mail-from sender@domain.tld --mail-rcpt recipient@domain.tld --upload-file body-email.txt
```

[Back to index](../../README.md)
