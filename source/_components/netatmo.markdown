---
layout: page
title: "Netatmo"
description: "Instructions how to integrate Netatmo component into Home Assistant."
date: 2016-06-02 08:10
sidebar: true
comments: false
sharing: true
footer: true
logo: netatmo.png
ha_category: Hub
ha_release: "0.2x"
---


The `netatmo` component platform is the main component to integrate all Netatmo related platforms. Besides this component you will have to setup any connected sensors separately.

To enable the Netatmo component, add the following lines to your `configuration.yaml`:

```yaml
# Example configuration.yaml entry
netatmo:
  api_key: YOUR_API_KEY
  secret_key: YOUR_SECRET_KEY
  username: YOUR_USERNAME
  password: YOUR_PASSWORD
```

Configuration variables:

- **api_key** (*Required*): The API key for your netatmo account.
- **secret_key** (*Required*): Your netatmo secret key
- **username** (*Required*): Username for the netatmo account.
- **password** (*Required*): Password for the netatmo account.

### {% linkable_title Get API and Secret Key %}

To get your API credentials, you have to declare a new application in the [NetAtmo Developer Page](https://dev.netatmo.com/). Sign in using your username and password from your regular NetAtmo account.
Click on 'Create an App' at the top of the page.

<p class='img'>
<img src='/images/screenshots/netatmo_create.png' />
</p>
You have to fill the form, but only two fields are required : Name and Description. It doesn't really matter what you put into those. Just write something that make sense to you. To submit your new app, click on create at the bottom of the form.

<p class='img'>
<img src='/images/screenshots/netatmo_app.png' />
</p>

That's it. You can copy and paste your new API and secret keys in your Home Assistant configuration file just as said above.

<p class='img'>
<img src='/images/screenshots/netatmo_api.png' />
</p>

<p class='note'>
The Home Assistant NetAtmo platform has only be tested with the classic indoor, outdoor module and rainmeter. There is no support for the windmeter module at this time because developers does not own these modules.
</p>
