# CT-WebSDK-React

## Introduction
This repository contains a sample project demonstrating the integration of CleverTap Web SDK with your website. The CleverTap Web SDK enables powerful user engagement and analytics capabilities for web applications.

## Prerequisites
Before you begin, make sure you have a CleverTap account. If you don't have one, you can [sign up for free](https://clevertap.com/signup) on the CleverTap website.

## Getting Started
To integrate CleverTap Web SDK into your website, follow these steps:

1. **Include CleverTap Web SDK**: Add the CleverTap Web SDK script to your HTML file's `<head>` section. Make sure to replace "886-85W-7Z7Z" with your CleverTap account ID.

```html
  <script type="text/javascript">
    var clevertap = { event: [], profile: [], account: [], onUserLogin: [], notifications: [], privacy: [] };
    clevertap.account.push({"id": "886-85W-7Z7Z"});
    clevertap.privacy.push({optOut: false}); 
    clevertap.privacy.push({useIP: true});
    (function () {
      var wzrk = document.createElement('script');
      wzrk.type = 'text/javascript';
      wzrk.async = true;
      wzrk.src = ('https:' == document.location.protocol ? 'https://d2r1yp2w7bby2u.cloudfront.net' : 'http://static.clevertap.com') + '/js/clevertap.min.js';
      var s = document.getElementsByTagName('script')[0];
      s.parentNode.insertBefore(wzrk, s);
    })();
  </script>
```

3. **Define Functions**: Define functions to handle user login, profile update, and event tracking.

```javascript
// Function to identify users on login
function OnUserLogin() {
  // Implement user identification logic
}

// Function to push additional user profile properties
function ProfilePush() {
  // Implement profile update logic
}

// Function to track custom events
function PDU() {
  // Implement custom event tracking logic
}

// Function to track charged events
function Charged() {
  // Implement charged event tracking logic
}
```

4. **Add HTML Forms**: Add HTML forms to trigger the defined functions.

```html
<!-- HTML forms for user login, profile update, and event tracking -->
```

5. **Handle Web Push Notifications**: Implement logic to handle web push notifications.

```javascript
// Function to request permission and show web push notifications
function pushNotify() {
  // Implement web push notification logic
}
```

6. **Run Your Website**: Refresh your Website and test the integration with CleverTap Web SDK.

## Resources
- [CleverTap Documentation](https://developer.clevertap.com/docs/web-quickstart-guide)
- [CleverTap Dashboard](https://dashboard.clevertap.com)
