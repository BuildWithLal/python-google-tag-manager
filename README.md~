#### [Google Tag Manager Python API](https://developers.google.com/tag-manager/api/v1/devguide)

Create javascript snippet code for your Google Tag Manager by providing your Site Name, Site URL
and Google Analytics Tracking code. This project creates [Universal Analytics](https://support.google.com/analytics/answer/2790010?hl=en) Tag so Tracking Code format must be like **UA-xxxxxx-xx**


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

##### Switch to project root directory and Install dependencies from requirements.txt file
```
pip install -r requirements.txt
```

##### What command do i need to execute?
```
# simply run from the command line
python index.py --site_name MY_SITE_NAME --site_url MY_SITE_URL --tracking_id MY_ANALYTICS_TRACKING_CODE
```

##### What do you get?
![Google Tag Manager Preview](https://lh3.googleusercontent.com/GvTbfvMvxSjJo_C24rfaLvvSftvmlTL0ZGHcrdU3y9LT_XDbIqwaJMNySpM-X_jTfjG_km_-FTqhhb0VjpAtHWVg5QeDLoPTymdYC3s5hT6WPM7ad0IADJW1ToHkLZLqTiks_h1HDoCYcYfmVjdcewy-OGnwYNeTRrLoeDEwchWG71iWS8nUFcmDNuaVYC8mXiptu-z1d6xfqsPcLWy2XUCbQdcq2vDg2F4zVFEasb5p4YCmfoYfLOVWFbtJOy3W7omJMICuHlr2AMnVpOvEMs3y-EgADBN5El5GtJSmJiDWr1uoeAl3rcC93ftCd2OLc7TTNtQdU4a8t1X_iPDYQ34FH6FEBaJCNnHINSwxQhkCHjWLxFxNXmjhE79WONnqxDeJ7U9pX7DmGuEM4LNbCeWr5ilz9B6uigL0xVd8NLmd9bxBl1luJVueVtSdFTwqSOLbsfD0eoQc71oN03f0n-06AR6XqDWMXMF9atOv7AiE0-6D4X23xEQJIvhrWeSLUi9V_qhyq3qNNWEqVA8uMO7cqm4KfMS8cDqu27EGIwqPjeJX_mY342RxHn2AIFMz9BEWomcUabvJZIz8C5nzDbEtD5diL5KJjefDg9H0cB3DXcAE=w1076-h581-no)

##### Tested Environment
```
Python 2.7
Python 3.4
Google Tag Manager API Version 1
Ubuntu 14.04
```