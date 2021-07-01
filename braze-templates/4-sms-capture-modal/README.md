<img alt="screenshot" src="screenshot.gif" height="500"/>

* Supports multiple country codes and validation
* Sets a phone number to the current user
* add "initialCountry: 'au'," as an argument to the intlTelInput javascript function to change the initial country.
``` javascript
var iti = window.intlTelInput(input, {
    nationalMode: true,
    hiddenInput: 'full',
    initialCountry: 'au',
    utilsScript: "https://appboy-images.com/appboy/communication/assets/code_assets/files/60ba5392f9088d62254859d1/original.js?1622823826"
});
```
