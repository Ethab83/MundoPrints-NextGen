---
id: wn8PE1RhG0znK1alrGFYv
title: Documentation
desc: "Homepage for all MundoCards Documentation"
updated: 1713669381290
created: 1631901573363
---

## Useful Links

- [MundoCards Homepage](https://mundocards.wpcomstaging.com/)
- [WordPress Dashboard](https://mundocards.wpcomstaging.com/wp-admin/)

## Scope

- **MundoCards Web-App**: A WP/WC SaaS web-app that facilitates on-demand printing services for consumers and local printers in emerging markets. The platform aims to aggregate consumer demand and automate the printers’ workflows through a SaaS web portal. The website should have a User-friendly UI and a secured payment API.
- **Consumer-end**: The business card designer software will be used to customize business cards that will be sold using the MundoPrints platform. The software will make it simple for customers to use MundoPrints from any device (mobile/desktop) easily.
- **Producer-end**: The printers/vendors will use a dashboard to manage their orders and product stock.

## Overview

This project (MundoCards), is for a Software Engineering class project at UMass Boston. Through the MundoCards platform, the user can customize their Business Cards according to their own requirements. Our task is to build an efficient website to incorporate as many customization features as we can for the business cards, 3-D views of the cards, and secured payment process.

## Limitations

Navigating the regulatory landscape across different countries can be challenging, with varying standards, taxes, and import/export regulations potentially complicating operations and expansion plans. One problem like this that we have run into was initially we were using a US-based WP website. However, we ended up switching this to an India-based WP website, because it was both cheaper, and more fitting. We will soon be implementing the payment system, and it will be important to make sure that the prices are shown in rupees instead of dollars.

Managing an efficient supply chain across diverse and sometimes remote areas can be complex, with risks of delays, increased costs, and logistical challenges affecting the timely delivery of services. This may not be much of a concern for us, since it will take too long to track the entire order fulfillment before the final deadline.

Managing the services, and website across different regions due to language barriers. Since the site is targeted towards the Indian market, it will be a challenge to make sure everything looks right.

Ensuring consistency with the product quality and packaging across all the different regions we are providing services to.

WP itself presents many limitations which are pay-walled behind subscriptions. We have run into several problems with limitations of some subscription levels, however with out current subscription, there are no further issues.

## Definitions

- UI: User Interface
- E-commerce: Electronic commerce
- WP: WordPress
- WC: WooComerce (e-commerce platform on top of WP)
- API: Application Programming Interface
- SaaS: Software as a Service
- MVC: Model, View, Controller
- iOS: iPhone OS (Operating System)

## Requirements

The most important requirement of this project is to create a user-friendly web-app that enables customers to customize their business cards according to their needs. To implement the website we are using WP.

The web-app must have a product navigation and customization UI for customers, and an orders dashboard for printing vendors.

The payment process must be smooth and secure for safety and reliability purposes. For this we are using WP plugins WC and RazorPay.

The website should be functional on all sorts of devices including a desktop or a phone(iOS/Android) Thankfully WP makes this fairly easy.
From the back-end perspective, the website should be able to connect the user with the local printers well, with all the order information and delivery notifications being sent to both parties at the same time. For this we are using the WP plugin called Zoho Campaigns.
Lastly, the website should also be able to track the details of the customers and store them in the database for future reference. For this we are using a WP plugin called JetPack.

## Specifications

The software will be implemented on a website (https://www.mundocards.com). It will be accessible from the homepage of it. The very first step in the process was to find out how we were going to build the website. We decided to use WP (with the Creator plan) because it could easily be used to implement the front-end design and add functionality through existing plugins. We copied the existing (unfinished) website. After obtaining the domain, we researched the specific plugins to implement (for payment processing, card customization, vendor dashboards, customer notification, etc.). Now, we are currently integrating the plugins to work seamlessly with the web-app.

## Design

We are first designing the actual UI and customization features with all the possible detailing to make the implementation of the front end easier. We are also coming up with the flow charts and discussing on the architecture and the required technologies to implement the back-end.

### Use Cases

The main clients of the software are small businesses and local printers in emerging markets. We connect small businesses to the local printers that are partnered with our site, allowing for operation sustainability. We’re also lookingto implement a phone application version of the website for Android/iOS, making it easier and more accessible to small businesses. The payment method implementation allows on-demand business card printing.

#### Actors

- **Customer**: A user who needs printing services and interacts with the website to create customized products, place an order, and pay for the order.

- **Local Printer Vendor**: A service provider who fulfills the printing orders placed by customers.
Use cases:

##### Customer Use Case

- **Sign Up**: New vendors register on the website to create an account with username and password.
- **Log In**: Old vendors access their accounts to manage their activities on the website.
- **Verify Password**: Part of the login process, the system validates user credentials.
- **Show Login Error**: If the login attempt fails, the system displays an error message to the user.
- **Customize Design**: Customers choose a design template or upload their own and personalize it with details like name, company information, etc.
- **Place Order**: Once the design is customized, the customer proceeds to place the order for printing.
- **Payment**: The customer completes the transaction by paying for the services through a secure payment gateway.
- **Manage Order**: Local printer vendors access the system to manage and process the orders received.
- **Receive Order**: After an order is processed, the local printer vendor updates the system, marking the order as complete when it’s ready for delivery or pickup.

### Architecture

We chose MVC architecture because it made the most sense for this application. The website is a type of online shopping platform, so it would be useful to have this architecture. The model in this case is a database to store information about customers and printers, as well as inventory, and available designs. As for deployment, it will be hosted on WP.

The exact implementation of the architecture is managed by WP. We chose WP because it made the most sense to copy the existing website (for other printed products) https://www.mundoprints.in/, to https://www.mundocards.com/ and change it to meet the requirements

### Technologies and Implementation Details

Since we are using WP most of the implementation will be inside WP and WP plugins. We are using the Elementor plugin to develop the front-end. Elementor is a drag and drop editor which makes it fairly easy to create a web UI. For managing products and customers we are using WC. For the design page we are using Zakeke which is a tailor made plugin for printing template customization. For the payment processing, we are using the RazorPay plugin for WP. For notifying customers for order confirmation and delivery, we are using Zoho Campaigns. For managing vendors and
implementing the vendor dashboard, we are using WC Vendors.

### User Interface

We based the User interface on MundoPrints.in which is still under development. Since MundoPrints.in has other products, we needed to remove the unneeded UI elements, and re-create the menu bar. This created unintended sideeffects, so we are currently working on making it smoother.

## Timeframe and Milestones

- By March 10th, we plan on receiving the existing codebase for the old website. This will be our next big milestone
as it will mark the start of our implementation phase.
    - We initially received the website on March 6th. However there were many limitations with the subscription plan, so after researching possible solutions and deciding that purchasing a higher-tier subscription through WP India. It wasn’t until March 22nd when we received access to the final website.
- By March 20th, we plan on completing R&D for the existing API’s and databases used, so that we can easily integrate them onto the new website.
    - We were able to research the existing WP plugins by this deadline, though there are extra plugins we have added and have just one more plugin to research.
- By April 25th, we plan on having a MVP for MundoCards.
