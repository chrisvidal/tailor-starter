# Settings

The Settings global blueprint is used throughout the backend and frontend to configure options throughout the theme. All settings are defined in the [`settings.yaml`](https://github.com/artistro08/tailor-starter/blob/main/seeds/blueprints/content/settings/settings.yaml) blueprint file

## Settings Tab

This tab allows you to do the following

* Set a Homepage from the [Pages ](pages/#index.htm)entry type
* Set The Website Name
  * Used in the meta tags throughout the pages
* Set a Favicon
* Set a Site Logo
  * Displayed in the Navbar
* Enable the Shop
  * If disabled, the Shop navigation item will be hidden.
  * Will also disable the products builder blocks
  * Will also disable the Currency, Stripe, and Shipping tabs on the page
* Enable Events
  * If disabled, the Event navigation item will be hidden.
  * Will also disable the events builder blocks
* Enable the Blog
  * If disabled, the Blog navigation item will be hidden.
  * Will also disable the posts builder blocks

> Note: if any of the switches are turned off on this page, you'll need to refresh the backend to see the changes.&#x20;

## Global Code Tab

This tab is used to place code snippets in their respective areas of the site.

## Currency Tab

Used in the [Shop](shop/), this tab is used to select the currency used in the shop. The currency code is used for [Stripe Checkout](https://stripe.com/docs/payments/checkout) to determine the current currency you want to charge people with.&#x20;

The Currency Symbol and Currency Symbol Placement options are cosmetics for the frontend of the site. They are not used in Stripe in any way.&#x20;

## Stripe Tab

This section contains placements for your Stripe keys and a Checkout Success page. **The Shop does not work unless you set everything on this page**.&#x20;

### Adding your Stripe Webhook Secret

The webhook secret is used to sign requests. The shop will not work without it. For step-by-step instructions on how to get it, [click here](https://scribehow.com/shared/Obtain\_a\_Stripe\_Webhook\_Secret\_\_5lTS37MMRnu\_hhGzWJe07w).

## Shipping

This section allows you to setup shipping on your site. It is also used in Stripe Checkout. Here's an explanation of each field below

### Countries to ship to

A list of country codes you would like to ship to. (Ex. US for United States, CA for Canada, etc.) [Find a country code](https://countrycode.org/)

### Shipping Methods

Allows you to add your own shipping methods that include price, and the min and max nubmer of days the package would arrive

## Mail Notifications Tab

This tab data is used to send you email notifications when a [Form](forms/) has been submitted, or when a [Product](shop/products.md) has been ordered. They are required when the Stripe Keys are set.&#x20;

## Forms Tab

This tab is used for reCAPTCHA keys. reCAPTCHA helps limit spam from forms in the backend. Only v2 is supported. You can get your keys [here](https://www.google.com/recaptcha/admin#list)