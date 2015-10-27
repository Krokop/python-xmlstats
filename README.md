# python-xmlstats
client for api https://erikberg.com/api

Work with python3.+


#Install
```bash
pip3 install python-xmlstats
```
#Use
Just init class, and send any request, low level.
```python
from xmlstats import XMLStats

stats = XMLStats(access_token='xxxxxxxxxxxxxxxxxxxxxxxxxxx', # access token you must get https://erikberg.com/api
                 email='some@email.com') #  email/website 
                                        #   to contact if there is a problem

responce = stats.make_request(host="erikberg.com", sport=None, method="events",
                              id=None, format="json",
                              parameters={'sport': 'nba', 'date':'20130414'})

```
# Hight level
##Get teams
```python
stats = XMLStats(access_token='xxxxxxxxxxxxxxxxxxxxxxxxxxx',
                 email='some@email.com')
teams = stats.get_teams()  # Return json https://erikberg.com/api/methods/teams
```

