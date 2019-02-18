---
description: >-
  Plans represent products and services you sell in Chargebee. Plans can be set
  up to have tiered pricing, free trials, additional products etc.
---

# Plans

Products and services must be effectively modelled in Chargebee for you to be able to bill your customers. _Plans_, along with other entities in the [_Product Catalog_](subscription-billing-guide.html#basic-setup) do just that. You would create plans in Chargebee with each of them corresponding to a specific product/service that your customers would subscribe to. Each Plan would, therefore, have associated with it information such as the Plan’s currency, pricing, billing interval etc.

For instance, you could be selling an online storage solution. While some users would intend to use the service for personal use, others may be business users. Hence, you could create say, a **home plan** that provides basic features and a higher priced **professional plan** for advanced features.

Your customers would be signed-up for plans by way of [_subscriptions_](subscriptions.html).

## Creating a Plan

Creating a new Plan for your business in Chargebee is quite simple. All you need to do is:

1. Log into your Chargebee web interface.
2. Go to **Product Catalog** › **Plans** › **Create a New Plan**.
3. In the _Create a New Plan_ page, enter all the necessary details about the plan. These are nothing but the basic plan attributes that form important component of a Plan. The upcoming section in this document will explain them in detail. 
4. Enable the _**This is a gift plan**_ checkbox while creating a plan to designate a plan to be used for signing up [gift subscriptions](gift-subscriptions.html). Also fill out [these additional details](gift-subscriptions.html#create-gift-plans) for such plans.
5. Once you are done, click **Save**, or to continue creating more plans, click **Save & Create New**. 

### Basic Plan Attributes

Plan attributes are the details that you enter about a plan and they are defined while creating or updating a plan. Let us look at each of these attributes in detail.

{% tabs %}
{% tab title="Plan Attributes" %}
| Plan Attributes | Description |
| :--- | :--- |
| Plan Name | It is the name used to refer to the plan on the Chargebee user interface. |
| Plan Id | It is the unique identifier of the Plan and when a Subscription is created or updated via the API from your app/website, the "Id" should be used to refer to the plan. |
| Invoice Name / Display Name | Name of the plan as it would appear to customers like say plan invoices, hosted checkout pages and customer portal and in quotes. |
| Plan Description | A short description to the plan for the customer. |

{% hint style="info" %}
#### Notes 

It's good to have a plan name that is descriptive of the attributes of the plan such as its pricing, billing period and currency so you can easily distinguish it from other plans in your site. So, instead of naming plans _Plan A_, _Plan B_ etc., it makes more sense to name them “Scale Yearly USD”, “Hustle Quarterly AUD“ etc.

If you don't set the invoice name, the plan name is used for it.

Plan description is shown in the [latest version](checkout-v3.html) of Checkout and Portal whenever the space available on the user interface permits. Other than in the latest version, it is shown only on the [change subscription page in Portal v2](customer_portal.html#change-subscription).
{% endhint %}
{% endtab %}

{% tab title="Billing Attributes" %}
| Billing Attributes | Description |
| :--- | :--- |
| Bill Every | The period or interval for which a single cycle of the plan is valid. Typically, while signing up, the customer pays for the first billing cycle and then again when the subscription to the plan renews at the end of the billing period. |
| Billing Cycles | The _No. of billing cycles_ determines the default number of times the subscription is renewed automatically. The number set should be inclusive of the first billing cycle. |
{% endtab %}

{% tab title="Accounting Attributes" %}
The Accounting information section helps Chargebee sync up with any accounting applications that you integrate with, like Xero and Quickbooks. Each of the accounting fields captures information that helps track product-specific sales/revenue from an accounting perspective.

| Accounting Attributes | Description |
| :--- | :--- |
| SKU | Store Keeping Unit is a name used to identify a product/service in inventory management or accounting systems. You can use this as an alternative name for your plan and it will be used as the _Product Name_ in the accounting system. |
| Accounting Code | This is a mandatory field that captures your Accounting systems' General Ledger Account code/name. When product information is synced to the Accounting system, the product-specific information will be synced with this account as captured here. |
| Accounting Category | This field captures product specific additional metadata or categorization for reporting purpose in the accounting systems \(such as regions you are selling to or branches you are selling from\). It should be entered in the format: _:. E.g. "Region: Northern”_ |
{% endtab %}
{% endtabs %}

