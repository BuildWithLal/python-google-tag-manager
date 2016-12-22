##### [Google Tag Manager Python API](https://developers.google.com/tag-manager/api/v1/devguide)

Create javascript snippet code for your Google Tag Manager by providing your Site Name, Site URL
and Google Analytics Tracking code. This project creates [Universal Analytics](https://support.google.com/analytics/answer/2790010?hl=en) Tag so Tracking Code format must be like **UA-xxxxxx-xx**

<br/>
##### Enable Google Tag Manager API
[Enable Google Tag Manager API](https://console.developers.google.com/start/api?id=tagmanager&credential=client_key)

<br/>
##### Make required changes in settings.py
```python
# enable/disable sending javascript code snippet in email.
SEND_CODE_SNIPPET_EMAIL = True

# SMPT settings goes here...

# secret key must be in /secrets/ folder. otherwise change directory here
# How to get secret key JSON file. Follow link
# https://developers.google.com/tag-manager/api/v1/devguide#environment

GOOGLE_DEVELOPER_SECRET_KEY = os.path.join('secrets', 'google_developer_secret.json')

TIME_ZONE_COUNTRY_ID = 'US'
TIME_ZONE_ID = 'America/Los_Angeles'

# possible values: web, android, ios
GOOGLE_TAG_USAGE_CONTEXT = ['web']
```

<br/>
##### Switch to project root directory and Install dependencies from requirements.txt file
```
pip install -r requirements.txt
```

<br/>
##### What command do i need to execute?
```
# simply run from the command line
python index.py --site_name MY_SITE_NAME --site_url MY_SITE_URL --tracking_id MY_ANALYTICS_TRACKING_CODE
```

<br/>
##### What do you get?
![Google Tag Manager Preview](http://i.imgur.com/nV4CFVl.png)

<br/>
##### Tested Environment
```
Python 2.7
Python 3.4
Google Tag Manager API Version 1
Ubuntu 14.04
```

