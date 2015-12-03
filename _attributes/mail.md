---
layout: page
title: mail
tags: [ attribute, mail ]
excerpt:
  The `mail` attribute
---

The `mail` attribute is defined in the [Cosine LDAP
Schema](https://tools.ietf.org/html/rfc4524#section-2.16). Normally
it's a multi-valued attribute containing a list of email addresses
associated with an LDAP object (account, person, etc), but at Stanford
it's only populated with a single value: the person's preferred email
address, set in StanfordYou.

## Stanford Email Addresses

Only full SUNetIDs have Stanford-provided email addresses; people with
base SUNetIDs can set their email address in StanfordYou, but it won't
be an @stanford.edu address.

People with full SUNetIDs technically have up to 3 SUNetIDs: the one
they created - which is used for logging in to systems and applications
- and up to two aliases. Email can be sent to any of those SUNetIDs,
but only one is published in the directory (this is controlled in
StanfordYou). The published email address is stored in the `mail`
attribute in the directory, and is released by Stanford's IdP as the
`mail` attribute.

Since people can change their aliases, or change which email address is
published, at any time, the `mail` attribute is not recommended as a
user identifier; [eppn] is a better choice.




