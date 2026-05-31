## Auto Login & OTP

Because my university's login page is so annoying.

## Installation & Usage:

Install [Tampermonkey](https://www.tampermonkey.net/) and then click [this link](https://raw.githubusercontent.com/pcider/auto-login-otp/refs/heads/main/sutd-auto-login.user.js) to install it.

By default, the script will not autofill values if you leave them blank in the script.

To use the autofill functionality, edit in the values shown below in `sutd-auto-login.user.js`. 
If your browser already autofills for you, you can leave it empty. (better to not put your passwords in scripts!)

You can access the script editor by clicking on Tampermonkey's icon (to the right of the URL textbox) > Dashboard > Auto Login & OTP. Now you can fill in the appropriate values.

```js
// leave empty if you dont want the script to autofill for you
const USERNAME = '<STUDENT_ID>';        
const PASSWORD = '<PASSWORD>';

// in your authenticator app, you should get a URL like
// "otpauth://totp/ease.sutd.edu.sg:<STUDENT_ID>?secret=<SECRET>&issuer=ease.sutd.edu.sg"
// input the <SECRET> part of the URL here.
// leave empty if you dont want the script to autofill for you
const TOTP_SECRET = '<SECRET>';
```
