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
