# Configuring Checkout

As a merchant, Chargebee provides you with a powerful configuration capability that you can use to build your checkout the way you want.

### Configuration Settings

To access the configuration screen click **Settings &gt; Configure Chargebee &gt; Checkout and Self Serve Portal.** You can configure the settings from this screen.

 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1544443040317_Screen+Shot+2018-12-10+at+5.27.02+PM.png)

{% hint style="info" %}
If you are a first time user and would like to use Chargebee Checkout enable the checkout to access the settings. 
{% endhint %}

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545897347324_Screen+Shot+2018-12-27+at+1.25.14+PM.png)

#### Show Legal Information

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545227920591_Screen+Shot+2018-12-19+at+7.26.58+PM.png)

You can choose to get consent or just display the Terms and Privacy links for your customers while they checkout.

\[Insert Video\]

#### Adding/Editing Quantity of Products

You can allow your customers can edit the quantity of products by enabling the settings shown in the screenshot below.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545646843394_Screen+Shot+2018-12-24+at+3.50.21+PM.png)

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545646869008_quantity.gif)

Merchants can also set a minimum and maximum quantity for their plans using meta configuration. [Learn more about this here](https://www.chargebee.com/docs/metadata.html). \[block:callout\] { "type": "info", "body": "In case you do not want your customers to edit the quantity of the plans, we’d recommend you not to enable the ‘**Allow customers to edit the quantity of plans**’ setting.", "title": "Note" } \[/block\]

#### Adding/Removing Coupons

Enable the ‘**Allow customers to add/remove coupons**’ setting in Chargebee in order to allow your customers to add/remove coupons. \[block:callout\] { "type": "danger", "body": "In order to add/remove coupons, the coupon field must first be configured. To configure that select **Settings &gt; Configure Chargebee &gt; Checkout & Self-serve portal &gt; Label.** Add **'Apply coupon’ and ‘Enter coupon code'** labels. Learn more about Labels.", "title": "Prerequisite for Displaying Coupons" } \[/block\] 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545648607199_Screen+Shot+2018-12-24+at+4.19.51+PM.png)

#### Editing/Removing Add-on

You can allow your customers to edit the quantity or the remove add-ons that you have added along with your plan. To know how to pass an add-on with a plan, refer to this link.

Enable the ‘**Allow customers to edit/remove addons’** setting to allow your customers to remove the add-on. 

{% hint style="info" %}
Quantity based add-ons can only be edited.\n- Customers cannot edit/remove mandatory add-ons if you have integrated via drop-in script. 
{% endhint %}

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545648559864_Screen+Shot+2018-12-24+at+4.18.54+PM.png)

#### Allow Customers to Access Checkout Via API Only

Enabling this option will disable all drop-in script links. In case you have used a drop in script in your site we recommend you to streamline your API workflow first and then enable this setting.

On enabling this option the **Grab code** link next to your plan will be disabled and the drop in scripts will stop functioning instantly. To use drop-in script again, disable this setting.

#### Allow Customers to Have Multiple Subscriptions

This allows your customers to create multiple subscriptions using the same payment details. 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545380347013_multiple-subscriptions.gif)

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545645788857_1.png)

#### Allow Guest Checkout

Enables customers to checkout as a guest. This option will be visible only for customers whose email address is associated with a customer ID. Your customers can check out without having to sign in to their account. Since the customer does not sign in a new customer will be created and the subscription will be associated to it leading to an instance where the same customer has 2 customer IDs in Chargebee. \[block:callout\] { "type": "info", "body": "Not applicable to users who have enabled Checkout via API.", "title": "Note" } \[/block\] 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545381194783_guestcheckout.gif)

#### Allow Customers to Checkout Without Payment Details

Chargebee enables you to allow your customers to complete their checkout without adding a payment method to their subscription. This functionality is built in order to offer a smooth checkout experience for your customers who are sceptical about adding a payment method to their subscription before actually trying the product/service.

The checkout without payment method feature enables you to:

* Offer a free trial for your customers without collecting a payment method.
* Have a Freemium plan that does not collect payment information during checkout.
* Offer a 100% discount or a coupon without prompting for a payment method.

This feature is protected using [Google Invisible reCAPTCHA](https://www.google.com/recaptcha/intro/v3beta.html) to stop spam checkouts by bots. To use this feature:

* Enable **Allow customers to check out without payment methods** option.
* Select when you'd like to apply this functionality from **Skip Payment method collection during checkout with** checkbox. Available options are **Full credit/discount coupons, Plans with free trials and Zero-dollar plans**.

![](https://www.chargebee.com/docs/assets/screenshots/images/chargebee-checkout-portal-v3/checkout-without-payment.png)

{% hint style="info" %}
This feature is applicable only for new subscriptions created through checkout.\n- In case you are using the checkout only to collect payment information from your customers, this option will not have any effect \(i.e payment information will be collected from all your customers\).\n- You can disable this setting any time you wish in the future. Once you disable it, all the new subscriptions \(free/trial/coupons\) created post disabling this option will require payment information during the checkout process itself.
{% endhint %}

Read the Frequently Asked Questions on Checkout without Payment Method.

### Publishing the Settings

Once you enable the necessary settings, you need to publish them. In case you don’t, they will be saved as a draft. Please do note that the changes that you make will be effective only after you publish. To publish click the **Publish** button in the top right corner.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545820286706_Screen+Shot+2018-12-26+at+4.00.22+PM.png)

### Previewing Checkout

Chargebee’s powerful Preview functionality allows you to view how the checkout and self-serve portal will look for your customers.

To preview check out:

* Click the **Preview checkout/self serve portal** link in the **Checkout & Self-Serve Portal** page.
* In the preview screen that opens select Checkout to preview checkout and Portal to preview portal. 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545925307679_Screen+Shot+2018-12-27+at+9.11.24+PM.png)

* Select the scenario that you’d like to view under **Preview settings**. You can view the checkout flow for new users and existing users.

### Disabling Checkout Settings

You can disable all the checkout settings at once by clicking the **Disable** button. Disabling will terminate all the actions pertaining to checkout immediately and your customers will not be able to access Chargebee checkout.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545897214055_Screen+Shot+2018-12-27+at+1.22.00+PM.png)

### Thank You Page

Saying thank you is an integral part in every customer interaction. Chargebee allows you to either pass a small thank you note at the end of the transaction or redirect them to a custom URL.

#### Adding Thank You Note

* Select **Settings &gt; Configure Chargebee &gt; Checkout and Self Serve portal &gt; Labels**.
* Click Add more copy/text and search for the term ‘**CLOSE**’. The search results will vary depending on the scenario \(for example: Extend subscription, Gift subscription etc\). 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545927256096_Screen+Shot+2018-12-27+at+9.43.58+PM.png)

* Add the appropriate label and edit the text. Learn more on [configuring Labels](doc:configuring-fields-and-labels) 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1545927367957_Screen+Shot+2018-12-27+at+9.45.50+PM.png)

* Your “Thank you” note will get added as shown in the image below. 

![](https://d2mxuefqeaa7sj.cloudfront.net/s_4A3FFA8F888C35EB418869697F87746173956EC228A99A26E2DADFD9030B77C8_1546425408447_Screen+Shot+2019-01-02+at+3.52.34+PM.png)

#### Thank You Page Redirection

You can choose to redirect your customers to a Thank you page in your site once they complete the payment. Thank you page redirection must be done at a plan level.

To do so:

* Open the plan in Chargebee
* Mention the URL in the Redirect URL box. Chargebee will redirect the customer to this URL once they complete the checkout.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/328e350-redirect.png",
    "redirect.png",
    930,
    475,
    "#fafafc"
  ]
  ```

    }

  \]

  }

  \[/block\]

{% hint style="danger" %}
The domain of the URL must be whitelisted in Chargebee for successful redirection. Learn how to whitelist a domain.
{% endhint %}

### Pixel Tracking

Pixel Tracking is used to track the actions of your visitors on your website and measure the conversion.

#### Facebook Pixel Tracking

Facebook Pixel is a code that collects information and helps you optimize Facebook ads, track conversions, and remarket to people who have already taken some kind of action on your website.

Learn how to set up [Facebook Pixel Tracking using Chargebee Checkout](https://support.chargebee.com/support/solutions/articles/232393-setting-up-facebook-pixel-tracking-if-i-m-using-chargebee-checkout-v3-)

#### Google Analytics Pixel Tracking

Google Analytics works by the inclusion of a block of JavaScript code on pages in your website. When users to your website view a page, this JavaScript code references a JavaScript file which then executes the tracking operation for Analytics. The tracking operation retrieves data about the page request through various means and sends this information to the Analytics server via a list of parameters attached to a single-pixel image request.

Learn how to set up [Google Analytics Pixel Tracking using Chargebee Checkout](https://support.chargebee.com/support/solutions/articles/232389-setting-up-google-analytics-if-i-m-using-chargebee-checkout-v3-)

### Integrations

Chargebee provides powerful integrations with top referral and affiliate marketing software.

Referral Marketing:

* [FriendBuy](doc:friendbuy) 
* [ReferralCandy](doc:referralcandy) 

Affiliate Marketing:

* [Refersion](doc:refersion-affiliate) 
* [LeadDyno](doc:leaddyno-affiliate)

