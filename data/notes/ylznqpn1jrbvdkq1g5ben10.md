
## Quick Links

- [MundoCards Homepage](https://mundocards.wpcomstaging.com/)
- [WordPress Dashboard](https://mundocards.wpcomstaging.com/wp-admin/)
- [Project Task Board](https://github.com/users/Ethab83/projects/1)

## Definitions

- **API**: Application Programming Interface
- **E-commerce**: Electronic commerce
- **iOS**: iPhone OS (Operating System)
- **MVC**: Model, View, Controller
- **MVP**: Minimum Viable Product
- **SaaS**: Software as a Service
- **UI**: User Interface
- **WC**: WooComerce (e-commerce platform on top of WP)
- **WP**: WordPress

## Scope

- **MundoCards Web-App**: A WP/WC SaaS web-app that facilitates on-demand printing services for consumers and local printers in emerging markets. The platform aims to aggregate consumer demand and automate the printers’ workflows through a SaaS web portal. The website should have a User-friendly UI and a secured payment API.
- **Consumer-end**: The business card designer software will be used to customize business cards that will be sold using the MundoPrints platform. The software will make it simple for customers to use MundoPrints from any device (mobile/desktop) easily.
- **Producer-end**: The printers/vendors will use a dashboard to manage their orders and product stock.

## Overview

This project (MundoCards), is for a Software Engineering class project at UMass Boston. Through the MundoCards platform, the user can customize their Business Cards according to their own requirements. Our task is to build an efficient website to incorporate as many customization features as we can for the business cards and secured payment process.

## Limitations

Navigating the regulatory landscape across different countries can be challenging, with varying standards, taxes, and import/export regulations potentially complicating operations and expansion plans. One problem like this that we have run into was initially we were using a US-based WP website. However, we ended up switching this to an India-based WP website, because it was both cheaper, and more fitting. We will soon be implementing the payment system, and it will be important to make sure that the prices are shown in rupees instead of dollars.

Managing an efficient supply chain across diverse and sometimes remote areas can be complex, with risks of delays, increased costs, and logistical challenges affecting the timely delivery of services. This may not be much of a concern for us, since it will take too long to track the entire order fulfillment before the final deadline.

Managing the services, and website across different regions due to language barriers. Since the site is targeted towards the Indian market, it will be a challenge to make sure everything looks right.

Ensuring consistency with the product quality and packaging across all the different regions we are providing services to.

WP itself presents many limitations which are pay-walled behind subscriptions. We have run into several problems with limitations of some subscription levels, however with out current subscription, there are no further issues.

## Requirements

The most important requirement of this project is to create a user-friendly web-app that enables customers to customize their business cards according to their needs. To implement the website we are using WP.

The web-app must have a product navigation and customization UI for customers, and an orders dashboard for printing vendors.

The payment process must be smooth and secure for safety and reliability purposes. For this we are using WP plugins WC and RazorPay.

The website should be functional on all sorts of devices including a desktop or a phone(iOS/Android) Thankfully WP makes this fairly easy.
From the back-end perspective, the website should be able to connect the user with the local printers well, with all the order information and delivery notifications being sent to both parties at the same time. For this we are using the WP plugin called Zoho Campaigns.
Lastly, the website should also be able to track the details of the customers and store them in the database for future reference. For this we are using a WP plugin called JetPack.

## Specifications

The software will be implemented on a website [MundoCards.com](https://mundocards.wpcomstaging.com/). It will be accessible from the homepage of it. The very first step in the process was to find out how we were going to build the website. We decided to use WP (with the Creator plan) because it could easily be used to implement the front-end design and add functionality through existing plugins. We copied the existing (unfinished) website. After obtaining the domain, we researched the specific plugins to implement (for payment processing, card customization, vendor dashboards, customer notification, etc.). Now, we are currently integrating the plugins to work seamlessly with the web-app.
