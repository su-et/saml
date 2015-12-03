---
layout: page
title: Salesforce
tags: [ app, salesforce ]
excerpt:
  How to configure Single-Sign-On (SSO) into your Salesforce instance using SAML
---

Salesforce supports two mechanisms for enabling SAML SSO for your
users: sending the user's Salesforce username (email address) in an
assertion, or sending a _Federation Id_ in the assertion, and setting
the appropriate value on each user object in your Salesforce instance.

Salesforce also supports two ways to send the username or _Federation
Id_: in the NameID, or in an attribute.

## Stanford Email Addresses

Only full SUNetIDs have Stanford-provided email addresses; people with
base SUNetIDs can set their email address in StanfordYou, but it won't
be an @stanford.edu address.

People with full SUNetIDs technically have up to 3 SUNetIDs: the one
they created - which is used for logging in to systems and applications
- and up to two aliases. Email can be sent to any of those SUNetIDs,
but only one is published in the directory (this is controlled in
StanfordYou). The published email address is stored in the _mail_
attribute in the directory, and is released by Stanford's IdP as the
_mail_ attribute.

Additionally, people can change their aliases, or change
which email address is published, at any time, so relying on email
addresses staying static is not ideal.

## eduPersonPrincipalName

People can change the SUNetID they use to login, but it's only allowed
in exceptional cases. Stanford's IdP exposes this SUNetID, suffixed
with _@stanford.edu_, as the _eduPersonPrincipalName_ attribute.


