---
description: >-
  You can integrate Livquik Payment Gateway with your Magento Store to accept
  payments from customers. It supports for Magento 2.x version.
---

# Magento

## **Prerequisites**

* Sign up for a IppoPay account.
* Generate the API keys from the [Livquik Dashboard](https://merchantapp.livquik.com) by navigating to Settings and then API Keys. You can use the Test mode keys for testing and later switch to Live mode keys when going live with the integration.

## Integration Steps

### Step 1: Install Extension

#### Installation Without Composer

* Download the code.zip file from the [latest release](https://livquik-assets.s3.ap-south-1.amazonaws.com/Plugins/livquik-magento.zip). Extract the zip.
* Place the code folder from Step 1 in your app folder. If you're performing an update, replace/overwrite the existing code folder.
* Enable and deploy the IppoPay module using commands
  * `bin/magento module:enable Livquik_PaymentGatway`
  * `bin/magento setup:upgrade`
  * ~~`bin`~~`/magento cache:flush`

### Step 2: Configure Magento Store

To configure your Magento store for Livquik Payments

1. Log into your Magento store.
2. Choose Stores on the Admin sidebar to the left. Now go to Settings > Configuration.
3. In the Configuration page, click on Sales on the left and choose Payment Methods.
4. In the Payment Methods page, navigate to Livquik.
5. Enter your test mode \[PUBLIC\_KEY] and \[SECRET\_KEY]. These can be generated from your [Dashboard](https://merchantapp.livquik.com).
6. Select Yes for the option Enabled.
7. Click Save Config. This activates your account in the Test Mode. You can use this account to make a few test payments to ensure a successful workflow.

**Note: In test mode, no real money is deducted from your account.**

### Step 3: Accept Live Payments

After testing your Magento store, when you are ready to accept live payments:

1. [Generate the \[PUBLIC\_KEY\] and \[SECRET\_KEY\]](https://merchantapp.livquik.com) in the Live mode on your Livquik Dashboard.
2. Enter the Live mode \[PUBLIC\_KEY] and \[SECRET\_KEY] in your Magento store.
