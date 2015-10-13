---
layout: page
title: SAML
---

While SAML is an acronym for _Security Assertion Markup Language_, SAML
is actually a markup language and a set of profiles and bindings for
exchanging SAML documents.

There are two common SAML login "flows": [SP](/glossary/sp/)- and
[IdP](/glossary/idp/)-initiated (also known as SP- and IdP-first). The former has been more
popular in higher education, while the latter is often used with
portals.


## SP-Initiated Login

In this flow a person - _Alice_ - using a web browser navigates to a
website. If Alice is not already logged into the site, when she either
clicks on a login link, or attempts to access a protected resource, the
SP will attempt to authenticate her.  To keep this example simple, let's assume that the SP 

Once the SP has determined which IdP to use, it sends a SAML
Authentication Request to the IdP.


## IdP-Initiated Login