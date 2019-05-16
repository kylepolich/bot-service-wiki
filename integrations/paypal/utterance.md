# Paypal Button

In order to create a `paypal utterance` you will need a `Production ID` in order to accept actual transactions, There is also a field for `Sandbox ID`, which is another ID provided by PayPal through the Developer's Dashboard located at `https://developer.paypal.com/developer/applications/`.

The `Sandbox` ID is for testing, and will not actually process the transaction posted.

On the Developer Dashboard, a little down from the top is a section titled, "REST API apps". Under this if there is already a Link pointing to an app, then you can get the IDs you need by clicking on that. At the top-right of the App Page there is a toggle switch for `Sandbox`, and `Live` - changing this will give you access to the associated ID.

Copy and paste this into the utterance config for `PayPal Button` in `DCS`, and everything should work accordingly. You will not be able to use a `production` `PayPal Button` without having the `Production ID`, and the same concept applies for `sandbox` as well.
