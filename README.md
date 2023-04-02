# Jays-Store
This project is an e-commerce website that uses Strapi as the backend system and React, MUI, and Redux for the frontend. It also utilizes [Stripe](https://stripe.com/gb) for payment processing.

## Getting Started
To get started, you will need to update the .env.example files in both the client and server folders with the relevant details. After updating these files, rename them to .env.

## Prerequisites
To run this project, you will need to have Node.js and npm installed on your machine.
You will also need to install Strapi for the Backend, so please do not copy across the whole folder from my code

## Installing Backend
First you want to set up your backend with [Strapi](https://strapi.io/) that has all the documentation you need to get started.
Once setup and you have ran the necessary commands in your terminal, you will now need to set up the data in the Strapi app.

To do this, you will need to use npm start in the server folder for the strapi app to initialise on localhost://1337 where you will sign up to get started.
Now you will see in the content builder you will already have the User set up, so now we need to set up the Order and Item categories.

First, let's start with the Order, as it is the easiet:
You will click on create new type and then type in Order with the following attributes:
  ##  NAME	     /       TYPE
    products            JSON
    userName            Text
    stripeSessionId     Text 

Then will want to create a new type called Item with the following attributes:
  ##  NAME	     /       TYPE
    name                Text 
    shortDescription    Rich text
    longDescription     Rich text
    price               Number
    image               Media 
    category            Enumeration 
    
Now once you have done that you can click on Content Manager, select Item and then add entry, this is where you will enter the images you wish to use to display your products.

## Installing Frontend
To install the dependencies, run the following command in the client folders:
npm install

## Running the project
npm start

## Stripe Payment
This project uses Stripe for payment processing. You will need to create a Stripe account and obtain your API keys. Update the .env files in both the client and server folders with your Stripe API keys.

## Built With
* Strapi
* React
* MUI
* Redux
* Stripe

## Acknowledgments
This project was created as part of a tutorial series on building e-commerce sites with Strapi and React.
