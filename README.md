passwick-api
=============

This README serves as the PassWick API documentation.




## Overview

The PassWick API gives your organization the ability to create and deliver Apple Passbook _passes_ to your customers.

## Connecting to the PassWick API

Before you can use the PassWick API you must register your organization at [PassWick](http://www.passwick.com).  You then use your PassWick username, password, organization ID and HTTP Basic Auth over SSL to connect to the PassWick APIs.

You will have the ability to:
* Create and edit your organization's Template Passes.
* Create, edit, and retrieve passes for your customers.
* Create passes with redeemable fields.
* Create links to your passes from your organization's web site.
* Deliver your organization's passes to your customers.

## Key Concepts

The most import concept to understand is **template pass**.  A template pass is a pass that you design using the PassWick Template Pass UI.  The template pass is the base used to deliver passes.  Think of a Template Pass as the model that describes the style, colors, content, and data fields for your organization's Passbook passes.  A customer pass is the realization of the template pass with any customer fields, like customer name, filled in for that customer.

Once you have designed and created a template pass you can then:
* Define the organizational data fields your template pass will display
* Define pass fields as redeemable
* Push notify your customer when pass data fields are updated
* Retrieve passes and deliver them using your organization's infrastructure.

## API Technology

PassWick uses RESTful web services and JSON over HTTPS.

####Template Pass

A *template pass* defines the style, color, and fields for your passes.  _At this time, Template Passes must be created using the PassWick Template Builder UI_

####Customer Pass

You can create a pass for your customer quite easily.  After you have built your template Pass and defined your organization's data fields you simply post a small JSON object to PassWick.

####Dynamic Pass Fields

With PassWick not only can you design your template passes with your organization's look and feel, you also get to decide what customer data will be displayed in the Passbook pass fields at design time. Customer data could be names, membership numbers, and even a thumbnail image of your customer.  The name that you give these data fields in the PassWick Template Builder UI is the same name that you use in the APIs.

## Security
Before you can use the PassWick API you must register your organization at [PassWick](http://www.passwick.com).  You then use your PassWick username, password, organization ID and HTTP Basic Auth over SSL to connect to the PassWick APIs.


## API Documentation

[The detailed API documentation can be found here](https://github.com/JasonD5150/passwick-api/wiki/API-Methods).


## Feedback

Please send questions or comments to jason@passwick.com. 

