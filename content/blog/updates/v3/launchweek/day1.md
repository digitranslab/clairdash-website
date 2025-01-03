---
title: Day 1 - Introducing our new data-first experience
description: Welcome to day one of Clairdash 3.0. We’ve reimagined the data experience from the ground up, introducing five powerful features that make it faster and easier than ever to build secure workflow apps. 
type: blog
layout: single
profilePic: https://res.cloudinary.com/daog6scxm/image/upload/v1699284176/Branding/Assets/Symbol/RGB/Full%20Colour/bb-symbol-trans_v60zdz.svg
images:
  - https://res.cloudinary.com/daog6scxm/image/upload/v1730364165/campaigns/3.0/day%201/day_1_light_b7c2kr.png
image: https://res.cloudinary.com/daog6scxm/image/upload/v1730364165/campaigns/3.0/day%201/day_1_light_b7c2kr.png
date: 2024-11-04
author: Mohamed BenChaliah
draft: false
---
{{< youtube id="zhKWphiOsPE" >}}


Welcome to day one of the Clairdash 3.0 launch week! Over the next few days, we’ll be diving into a variety of exciting new developments, each designed to enhance the way you build and manage your apps. Each day, we’ll explore a different theme, offering insights and guidance to help you get the most out of Clairdash 3.0.

*But let’s not get ahead of ourselves! We’re kicking off the week by diving into the new data experience in Clairdash.*

## New data-first experience

Every great application starts with a strong foundation—its data. In Clairdash, the Data section is your starting point for building powerful apps and lays the groundwork for everything that follows. 

With this in mind, we’ve reimagined the data experience from the ground up, introducing five powerful features that make it faster and easier than ever to build secure workflow apps:

1. [Enhanced Views](#enhanced-views)
2. [Default Values](#default-values)
3. [Row Actions](#row-actions)
4. [View Joins](#view-joins)
5. [Dynamic Screen Generation](#screen-generation)


## Control access with Enhanced Views {#enhanced-views}

Controlling who can view, access, and manipulate data is crucial to building secure applications in Clairdash. 

That’s why with Clairdash 3.0, we’ve completely overhauled Views, making them the primary way permissions and access are defined in Clairdash. You can now set up a new view for each role using your application, and seamlessly control what data they can see and manipulate. 

By starting in the data section, we ensure a secure-by-design approach to managing access and permissions, making security step one in application development—not an afterthought.

For example, imagine a typical approval workflow with two roles: a `Submitter` and an `Approver`.

A `Submitter` should be able to:
- Create a new request.
- View, edit, and cancel their own requests.
- Not see other users' requests or approve/reject requests.

An `Approver` should be able to:
- View all requests.
- Approve, reject, or cancel requests.
- Not see unsubmitted draft requests.

To keep things simple, we’ll just set up the `Approver` role for now, but we’d take the exact same approach for the `Submitter` role, too. The custom roles have already been created for this example, so let’s jump straight in and create a new `Approver` view. 

![Create new view](https://res.cloudinary.com/daog6scxm/image/upload/v1730408170/campaigns/3.0/day%201/create_view_iprydq.webp)

Then, set the access level for the view to the `Approver` role. 

![Views access](https://res.cloudinary.com/daog6scxm/image/upload/v1730408168/campaigns/3.0/day%201/custom_roles_t3bloc.webp)

We’ll set up a filter on our table to ensure that the `Approver` can only access requests to which they’ve been assigned. For this example, we’re checking that the `Approver` email column matches the email of the `currently logged-in user` to Clairdash.

![View filter](https://res.cloudinary.com/daog6scxm/image/upload/v1730408485/campaigns/3.0/day%201/filter_peddpe.webp)
With Views, you can then customize and manage role permissions effortlessly. Use filters to control which rows each role has access to, or assign permissions to each column—edit, read-only, or hidden.

![View columns](https://res.cloudinary.com/daog6scxm/image/upload/v1730408168/campaigns/3.0/day%201/columns_kksh6t.webp)

You can create as many Views as you want, which you can easily toggle between using the tabs above. 


> **Previous to this release, View Access Configuration was a paid feature. With 3.0, this is now a free feature for all Clairdash users.**


---

## Set Default Values {#default-values}

![Default values](https://res.cloudinary.com/daog6scxm/image/upload/v1730382869/campaigns/3.0/day%201/Default_valuesportrait_pr8o6r.webp)

Default values offer a streamlined experience for gathering data. You can set columns to a dynamic or static value when a new entry is created. For example, you can set the default value to `In progress`, `Current employee`, or the `Date` of a record's submission. Default values eliminate the need for repetitive manual data entry, and ensure that information collected automatically is accurate and consistent.

![Default values](https://res.cloudinary.com/daog6scxm/image/upload/v1730408167/campaigns/3.0/day%201/Default_values_date_u4mje1.webp)


---

## Streamline data workflows with Row Actions {#row-actions}

![Row Actions](https://res.cloudinary.com/daog6scxm/image/upload/v1730407457/campaigns/3.0/day%201/Row_actions_zhc8le.webp)

Row Actions link automations to your data, creating data-driven workflows that are both easy to set up and secure by design. This feature allows you to assign different actions to different users on the same dataset.

For example, in an approval workflow, an approver can `Approve` or `Reject` a request, while a submitter can `Edit` or `Cancel` it. This can be set up as four different row actions (aka automations), with each action only shown to the correct job role.

Let’s see how to set up the Approve action:

{{< vimeo id="1025386963" title="Row Actions" >}}

This targeted approach lets users take specific actions on a table, such as approving a request without full access to make unrestricted changes. By controlling user actions, Clairdash 3.0 enhances the usability and security of your applications, simplifying automation creation and role management.

---

## Connect data with View Joins {#view-joins}

![View Joins](https://res.cloudinary.com/daog6scxm/image/upload/v1730409505/campaigns/3.0/day%201/view_relationships_mjtaun.webp)

View Joins allow you to display related data from other tables directly in your views, streamlining workflows, enhancing data visibility, and providing more ways to manage data security. 

For instance, in an approval app, we might want to set up a relationship between the `Requests` and `Approvers` views. This way, using View Joins, we can easily pull in columns like the Approver's name or email and show them directly in the Requests view without modifying your schema.

Related data, such as the employee's name, is always view-only, preserving security while providing essential context. View Joins will also only display data from the immediately related table, keeping your views clean and manageable.

---

## Dynamic Screen Generation {#screen-generation}

For our fifth and final feature today, we’re covering Dynamic Screen Generation.

You’ll now notice a new Generate button in your data section—this is where the magic happens. With the click of a button, generate fully-working apps and forms from the data you're currently working with.

*With just a click, generate screens from your Views and watch them come to life in seconds!*

{{< vimeo id="1025386944" title="Generate Screen" >}}



---

## This is just the beginning

We hope you’ve enjoyed today’s release! As we’ve explored today, Clairdash 3.0 empowers you to build more secure, data-driven applications with ease. 

From Dynamic Views that control role-based access to powerful new features like Automatic Screen Generation, the enhanced data experience streamlines app development and elevates what you can achieve with the platform.

Throughout the week, we'll be unveiling more features that will transform your app-building journey. Tomorrow, we'll explore Role-Based Access Control, reinforcing our commitment to secure-by-design app development.

Try out the new features above by logging into your Clairdash account or [signing up](https://account.clairdash.app/register).