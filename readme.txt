=== XpertCreation Pi Network Payments for WooCommerce ===
Contributors: khalidxpert
Tags: pi network, pi payment, cryptocurrency, woocommerce, payment gateway
Requires at least: 5.0
Tested up to: 7.0
Requires PHP: 7.4
Stable tag: 1.0.0
Requires Plugins: woocommerce
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Accept Pi Network cryptocurrency payments in your WooCommerce store. This plugin is not officially affiliated with Pi Network or WooCommerce.

== Description ==

**XpertCreation Pi Network Payments for WooCommerce** is a payment gateway plugin that enables WooCommerce store owners to accept Pi Network cryptocurrency payments at checkout.

This plugin is developed by XpertCreation and is not officially affiliated with Pi Network or WooCommerce/Automattic.

= Features =

* Accept Pi Network payments at checkout
* Easy setup - add your Pi App ID and API Key from Pi Developer Portal
* Sandbox/Testnet mode for testing before going live
* Automatic payment verification via Pi Network API
* Order status auto-update after payment confirmation
* Live Pi exchange rate support via CoinGecko API
* Mobile friendly - works in Pi Browser

= How it works =

1. Customer adds products to cart
2. At checkout, customer selects "Pay with Pi Network"
3. Customer authenticates with Pi Network in Pi Browser
4. Payment is created and verified automatically
5. Order is completed and customer is redirected to thank you page

= Requirements =

* WordPress 5.0+
* WooCommerce 5.0+
* PHP 7.4+
* Pi Network Developer Account
* Pi App ID and API Key from developers.minepi.com

== External Services ==

This plugin connects to the following external services:

= Pi Network API (api.minepi.com) =

This plugin connects to the Pi Network Platform API to approve and complete payments made by customers using Pi cryptocurrency.

* **What is it:** Pi Network's official payment processing API
* **What data is sent:** Payment identifier, transaction ID, and your Pi API Key (server-side only)
* **When is it sent:** When a customer initiates a payment, when approving a payment, and when completing a payment
* **Pi Network Terms of Service:** https://minepi.com/terms-of-service
* **Pi Network Privacy Policy:** https://minepi.com/privacy-policy

= Pi Network SDK (sdk.minepi.com) =

This plugin loads the Pi Network JavaScript SDK on the checkout page to handle user authentication and payment flow in Pi Browser.

* **What is it:** Pi Network's official JavaScript SDK
* **What data is sent:** User authentication data handled by Pi Browser
* **When is it sent:** When the checkout page loads and when a customer authenticates
* **Pi Network Terms of Service:** https://minepi.com/terms-of-service

= CoinGecko API (api.coingecko.com) =

This plugin optionally connects to CoinGecko to fetch the live Pi Network exchange rate in USD.

* **What is it:** A cryptocurrency price aggregation service
* **What data is sent:** No personal data is sent. Only a public API request for Pi Network price data
* **When is it sent:** When calculating Pi payment amounts based on your store currency
* **CoinGecko Terms of Service:** https://www.coingecko.com/en/terms
* **CoinGecko Privacy Policy:** https://www.coingecko.com/en/privacy

== Installation ==

1. Upload plugin to `/wp-content/plugins/pi-pay-for-woocommerce/`
2. Activate the plugin through 'Plugins' menu
3. Go to WooCommerce > Settings > Payments > Pi Network Payment
4. Enter your Pi App ID and API Key from developers.minepi.com
5. Enable sandbox mode for testing
6. Save settings

== Frequently Asked Questions ==

= Where do I get Pi App ID and API Key? =

Register at [Pi Developer Portal](https://developers.minepi.com) and create a new app to get your credentials.

= Does it work with Pi Testnet? =

Yes! Enable Sandbox mode in settings to use Pi testnet for testing before going live.

= Is this an official Pi Network plugin? =

No. This plugin is developed by XpertCreation and is not officially affiliated with Pi Network or WooCommerce.

= What currencies are supported? =

Pi amount is calculated based on your WooCommerce store currency and the live Pi exchange rate from CoinGecko.

= Is it secure? =

Yes. All payments are verified server-side using Pi Network API before order completion. Your API Key is stored securely in WordPress options and never exposed to clients.

== Screenshots ==

1. Checkout page with Pi Network payment option
2. Pi authentication popup in Pi Browser
3. Plugin settings page in WooCommerce
4. Order confirmation page

== Changelog ==

= 1.0.0 =
* Initial release
* Pi Network payment gateway integration
* Sandbox/Mainnet support
* Automatic payment verification
* CoinGecko live rate support

== Upgrade Notice ==

= 1.0.0 =
Initial release.
