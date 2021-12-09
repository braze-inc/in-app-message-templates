> ⚠️ Note: Subscription Groups were introduced in Android SDK v15.0.0, Web SDK v3.4.0, and iOS SDK v4.3.3. Please ensure your SDKs are up to date, or apply filters to your message's targeting.

<img alt="screenshot" src="screenshot.gif" height="500"/>

* Supports multiple country codes and validation
* Sets a phone number to the current user
* To set the initial country, add `initialCountry: 'au'` as an argument to the `intlTelInput`:
``` javascript
var iti = window.intlTelInput(input, {
    nationalMode: true,
    hiddenInput: 'full',
    initialCountry: 'au',
    utilsScript: "https://appboy-images.com/appboy/communication/assets/code_assets/files/60ba5392f9088d62254859d1/original.js?1622823826"
});
```
