To [generate](https://alexcabal.com/creating-the-perfect-gpg-keypair/) a cryptographic key pair:

```bash
gpg ‐‐gen-key
gpg --edit-key me
> addkey # RSA (sign only), 4096, 0
> save
```

Export public key to [publish](http://www.gushi.org/make-dns-cert/HOWTO.html):

```bash
gpg --armor --output pubkey.txt --export me
```

Generate detached signature:

```bash
gpg --armor --output index.html.asc --detach-sig index.html
```

Use the following to [verify](http://www.gnupg.org/gph/en/manual/x135.html) that the HTML file is authentic.

```bash
gpg --verify index.html.asc index.html
```
