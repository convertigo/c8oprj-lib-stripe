# lib_Stripe
This is the Stripe payment platform Connector for Convertigo. This enables Convertigo Mobile or Desktop apps to interact with the Stripe platform for building __eCommerce__ or __mCommerce__ applications to accept payments.

# Installation

* In your Convertigo Studio use File->Import->Convertigo->Convertigo Project and hit the 'Next' button

* In the Dialog 'Project remote URL' field Paste :

        lib_Stripe=https://github.com/convertigo/c8oprj-lib-stripe.git

* And click the 'Finish' button

# Usage

## Configuring your Stripe Environment

Stripe needs you to configure some account information to get your API keys. You can find them in the Stripe dashboard :

    https://dashboard.stripe.com/test/dashboard

## Configuring Convertigo Symbols

__lib_Stripe__ needs some symbols to be configured. You configure them trough the Web Console: https://&lt;your site&gt;.convertigo.net/admin, hit the ___symbols___ button to get to the symbol configuration page.


Symbol  | value
------| ------
lib_Stripe.privateApiKey.secret | The private Stripe API Key you will find in the Stripe dashboard
lib_Stripe.publicApiKey | The public Stripe API  you will find in the Stripe dashboard.

## Shared Component

To enable Stripe payments in your app, you just have to insert the __StripeCreditCardPayment__ shared component in a page of your app. This will automatically show a Credit card form where customers can input their Credit Card number and Hit 'Pay'.

The Component will handle all the dialog with the Stripe platform, perform necssary checks and end with a payment confirmation or an error.


## Sample Application

You will find in this project a sample application using the __SAMLLogin__ shared component. Be sure to configure your IDP and the Convertigo symbols accordingly to run the app.


