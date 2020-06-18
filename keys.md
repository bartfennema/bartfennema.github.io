---
layout: page
title: My Keys
permalink: /keys/
---

I use [GnuPG](https://gnupg.org/) for email encryption and signing. I also use
it to sign various other things, such as documents, code, and this blog.

## The Master Key..

All my keys are signed by the following Master Signing Key:

pub   dsa1024 2006-05-23 [SCA]
      E1C181834E797F92FE8F69C1A094788ECE0C9C0E
uid           [ultimate] Bart Fennema <bfennema@gmail.com>
sub   elg4096 2006-05-23 [E]
sub   rsa4096 2020-06-18 [S]

This key is also attached to this repo in the [key/](/keys/) directory. You
should verify the fingerprint of this master key using some other channel than
just this blog.
I use this key for signing my blogposts as well.

* This key is attached here: [keys/bfennema.asc](/keys/bfennema.asc).

## Email encryption keys

The following is my GPG key for Protonmail:

pub   rsa2048 2015-05-11 [SC]
      D3D2DE04F43D9AA9041BED522EE1A0A50FF63062
uid           [ultimate] bartf1969@protonmail.com <bartf1969@protonmail.com>

* This key is attached here: [keys/bartf1969protonmail.asc](/keys/bartf1969protonmail.asc).


## Note on lack of expiration date on code-signing keys

My signing keys do not have expiration dates. This is not laziness. There is a fundamental problem with using an expiration date on keys used for code signing (e.g. `git tag -s`), because it
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


