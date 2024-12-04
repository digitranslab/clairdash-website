+++
author = "Mohamed BenChaliah"
date = 2022-03-14T00:00:00Z
description = "Clairdash’s public API is now publicly available - making Clairdash the hub for all your internal apps"
image = "https://res.cloudinary.com/daog6scxm/image/upload/v1647258318/cms/Start_building_with_Clairdash_s_API_bum2mr.png"
profilePic = "https://res.cloudinary.com/daog6scxm/image/upload/v1647258452/cms/20200113_Propel_Team_Shots_123_omblqt.jpg"
title = "Clairdash’s public API is now available"

+++

Today, we are launching one of our most requested features - our new public API!

When you sign up for Clairdash, you get a low-code platform with an internal database, external data connectors (MySQL, PostgreSQL, MSSQL, Oracle DB, Airtable, MongoDB…), user management, free SSO, drag and drop GUI for building UIs, powerful prebuilt components, free SSO, an automation interface (like Zapier) and now a flexible public API to interact with.

These services integrate very well with each other making the experience of building CRUD apps easier, faster, and a lot more flexible.

As with anything that we build in Clairdash, our new public API is simple to use, flexible, and introduces new extensibility. To summarize, the Clairdash API enables:

1. Clairdash as a backend  
   The Clairdash backend is very powerful, and our Public API allows you to specifically use the backend API to build apps, without using, for example, our design GUI. A common use case would be to pair the Clairdash backend with Grafana to build powerful dashboards, or to [use Clairdash with a frontend framework](https://clairdash.com/blog/building-a-crud-app-with-clairdash-and-next.js/ "use clairdash with a frontend framework"). The number of potential use cases are vast.
2. Extending apps  
   Right now users are limited to what you can do within Clairdash. This can make it difficult to extend functionality in a lot of places, especially around data. The new Clairdash API allows users to build to a point within Clairdash and then extend using the API. This is only the beginning, as Clairdash continues to grow we will improve and expand the capabilities of our API.
3. Inter-operability  
   Again right now for inter-op within an organization, you're limited to what Clairdash can connect to. Opening up the API allows connecting data in and out of Clairdash in ways that are business-specific use cases (e.g. IoT, internal business APIs, etc).

## Design

The API follows RESTful patterns of design and is fully defined using the OpenAPI specification. For schemas and API definitions this enables the spec to be pulled into tools like Postman and you can start making requests straight away once you've inputted your API key and App ID.

The first version of the API covers the tables, rows, users, queries, and applications resources. You have full CRUD operations on those resources as well as the ability to search any of them. This also respects the RBAC system fully. Every user can generate an API key for Clairdash and it will only allow users with access to resources to utilize the API.

## Use case

To help you adopt the Clairdash API, we’ve created the following example:

1. [Build an app with Clairdash and Next.js](https://clairdash.com/blog/building-a-crud-app-with-clairdash-and-next.js/)

## Docs

You can learn more about the Clairdash API at the following places:

1. [General documentation](https://docs.clairdash.com/docs/public-api): Learn how to get your API key, how to use spec, and how to use with Postman
2. [Interactive API documentation](https://docs.clairdash.com/docs/public-api): Learn how to interact with the API