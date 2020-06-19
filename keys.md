---
layout: page
title: My Keys
permalink: /keys/
---

I use [GnuPG](https://gnupg.org/) for email encryption and signing. I also use
it to sign various other things, such as documents, code, and this blog.

## The Master Key..

All my keys are signed by the following Master Signing Key:

    pub   rsa4096 2020-06-19 [SC]
          F45C36E8349987AB95B8ED1D63B69F001C4FB07B
    uid           [ultimate] Bart Fennema Master Key (Bart Fennema Master Key)
    sub   rsa4096 2020-06-19 [E]

This key is also attached to this repo in the [key/](/keys/) directory. You
should verify the fingerprint of this master key using some other channel than
just this blog.

* This key is attached here: [keys/BFmasterkey.asc](/keys/BFmasterkey.asc).

## Email encryption keys

The following is my GPG key for Protonmail:

    pub   rsa2048 2015-05-11 [SC]
          D3D2DE04F43D9AA9041BED522EE1A0A50FF63062
    uid           [ultimate] bartf1969@protonmail.com <bartf1969@protonmail.com>

* This key is attached here: [keys/bartf1969protonmail.asc](/keys/bartf1969protonmail.asc).


## Blog signing key

    pub   rsa4096 2020-06-19 [SC]
          3AC7982A172118C9CFA5831756723BF0DDF6A257
    uid           [ultimate] bartblog (Key to sign blogposts)
    sub   rsa4096 2020-06-19 [E]

* This key is attached here: [keys/bartblog.asc](/keys/bartblog.asc).

## Note on lack of expiration date on code-signing keys

My signing keys do not have expiration dates. This is not laziness. 
There is a fundamental problem with using an expiration date on keys used for code signing (e.g. `git tag -s`), because it
is unclear what the outcome should be when one verifies some old code (written
and signed when the key was still valid) in the future when the key has already
expired?

Naturally we would like the old code, written and signed when the key was still
valid, to continue to verify fine also in the future, after the key expires
(and the developer passed away, perhaps).  However, it is very problematic to
prevent the attacker from creating falsified code pretending to be an old one.


## Other keys

There is no bunch of other keys in the
[keys/](https://github.com/)
directory -- these are implicitly signed by my master key by being part of this
(tag-signed) repo.


## Other notes

* I proudly use empty passphrases on all of my private keys. This is because if
somebody was able to execute malicious code in the VM where a private key
lives, then the key should be considered compromised no matter how complex
passphrase I used to protect it.  Passphrases on private keys are classic
example of [Security Theater](http://en.wikipedia.org/wiki/Security_theater) in
my opinion.  O.o ... huh! ... I like Joanna's opinion on security;


