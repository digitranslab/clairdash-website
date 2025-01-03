+++

date = "2021-07-25"
title = "July 2021 release - SSO, conditional UI, and more"
description = "The July release delivers on a number of popular requests from our community and contains four major updates, including; SSO, conditional UI, dark mode apps, SQL relationships."
author = "Mohamed BenChaliah"
images = ['/releases/2021/june/layout.png']
draft = "false"

+++

 {{< youtube LJHA2K8loaw >}}

The July release delivers on a number of popular requests from our community and contains four major updates, including;

1. SSO - OIDC support
2. Conditional UI
3. Themeable apps
4. Map SQL relationships within the builder

---

### SSO - OIDC support

OIDC is an open standard and decentralized authentication protocol. As a user, you will have infinite possibilities for SSO, including:

- Active Directory! - popular request
- Auth0
- Azure
- Okta
- OneLogin
- It’s also possible to add your own authentication! 

I know many of you will understand the benefits of SSO, but here’s a quick recap:

- No more password management
- Auto-provisioning for users
- Minimize password security risks
- Quicker sign up/sign-in process for users
- Use your SSO provider to control who can access Clairdash

The initial work for this feature was completed by community member, [Bernhard Hayden](https://github.com/burnoutberni). We’d like to publicly thank Bernhard for taking the time and effort to contribute to Clairdash. The remaining work was completed by two new Clairdash recruits; [Peter](https://github.com/PClmnt) and [Rory](https://github.com/Rory-Powell).

### Conditional UI

When building apps with Clairdash, you will now have the ability to change your UI depending on the state of the application. This new feature allows you to hide content from certain users, change the color of text depending on its value, and more.

### Dark mode apps 

We strive to make it as easy as possible for you to build beautiful, user-friendly internal tools with Clairdash. After this release, switch between 4 themes for your apps; lightest, light, dark, darkest, with just 2 clicks.

### SQL relationships

Import tables from your SQL databases (with just 1 click), then map relationships between your tables within Clairdash. This allows you to utilize the power of relationships within your Clairdash applications. 

## Additional updates

- Unauthenticated SMTP
- Clairdash drawer UI improvements
- [Layout update](https://github.com/Clairdash/clairdash/pull/1969)
- Lucene search improvements

## Coming up in the August release

- Dynamic forms and a Wizard component
- A better developer experience (JavaScript, transformers, and auto-complete)
