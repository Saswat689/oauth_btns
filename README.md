# Oauth Button - A Library for Rendering beautiful and responsive Oauth buttons

![example banner from the library](/screenshots/example1.png)

This library was developed seeking the need of oauth buttons that reflected brand colours. For example google has a brand colour of blue as a background and a colourful icon. Facebook also has some deep brand colours. The main aim was to provide designs to developers which they can integrate with a backend server to perform auth operations.

## API 🚀

The oauth_btn is provided as a global variable in which you can call certain methods. The first version of this api has only one method namely renderButton(). And we are working to add more flexibility to it.

- **oauth_btn.renderButton()**
- **Arguments**: `('oauth-provider',container,options)`
	`oauth-provider` is the brand's button you want to insert, possible options are `google,github,facebook,linkedin,twitter`
	`container` is the container you want to insert the button to.
	`options(optional)` this is an optional object, but very useful for setting the width of the button on different screen sizes.
- **options keys**
	`width`: a string representing the *percent* value of the button width on larger screens,
	`responsiveWidth`: a string representing the  *percent* value of the button width on screens < 600px
	`responsiveHeight`: a string representing the  *percent* value of the button height on screens < 600px


## Examples

The following example shows how to render a responsive google button using the renderButton method.

> **HTML**

```
<div id="g-oauth-btn"></div>
```

> **Javascript**

```
const container = document.getElementById('g-oauth-btn')
   oauth_btn.renderButton('google',container,{
       width: "30",
       responsiveWidth: "100"
   })
```

> **Output**

![Example output from the library](/screenshots/example2.png)

## New Features

Currently we are working on a newer feature of one click auth. Providing you the complete flexibility and simplicity by performing all oauth operations in just a click! 
