### passlib
---
https://passlib.readthedocs.io/en/stable/

```py
from passlib.hash import pdkdf2_sha256

hash = pdkdf2_sha256.hash("toomanysecrets")
hash

pdkdf2_sha256.verify("toomanysecrets", hash)
pdkdf2_sha256.verify("joshua", hash)

from passlib import totp
otp = TOTP(key='xxx')
otp.match('359', time=1475338840)

otp.match('123456', time=147338840)
otp.match('359275', time=1475338840)


from passlib.hash import hex_sha1 as hex_sha1
h = hex_sha1.hash("password")
h

hex_sha1.verify("password", h)
hex_sha1.verify("secret", h)
```

```
```

```
```


