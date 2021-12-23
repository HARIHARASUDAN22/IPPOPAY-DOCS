---
description: >-
  Livquik payment gateway plugin for CS-Cart. Allows merchants to accept
  payments with the CS-Cart store. It uses a seamless integration.
---

# CS Cart

### Livquik Payment Extension for CS Cart

Allows you to use Livquik payment gateway with the CS Cart Store.

### Description

​This is the Livquik payment gateway plugin for CS Cart. Allows merchants to accept payments with the CS Cart store. It uses a seamless integration, allowing the customer to pay on your website without being redirected away from your CS Cart website.

### Installation

1. Ensure you have latest version of CS Cart installed.
2. [Download](https://livquik-assets.s3.ap-south-1.amazonaws.com/Plugins/livquik-cscart.zip) the zip of this repository.
3. Inside the file downloaded above is a file called 'install\_livquik.sql'. This has to be executed against your cscart database. You can use phpmyadmin to import the file into your cscart database or copy paste the content and run directly into your mysql shell.
4. Upload rest of the contents of the plugin to your CS Cart Installation directory (content of app folder goes in app folder, content of design folder in design folder).

### Configuration

1. Log into CS-Cart as administrator&#x20;
2. Navigate to Administration / Payment Methods.
3. Click the "+" to add a new payment method.
4. Choose Livquik from the list and then click save. For template, choose "cc\_outside.tpl"
5. Click the 'Configure' tab.
6. Enter your Livquik Public Key and Secret Key which you can get from Livquik Dashboard.
7. Click 'Save'

#### Support

Visit [https://livquik.com](https://livquik.com)  for support requests or email techsupport@livquik.com.

