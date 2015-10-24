# python-xmlstats
python module for https://erikberg.com/api

#Install
```bash
pip3 install python-xmlstats
```
#Use
```python
from xmlstats import XMLStats

stats = XMLStats(access_token='xxxxxxxxxxxxxxxxxxxxxxxxxxx', # access token you must get https://erikberg.com/api
                 email='some@email.com') #  email/website 
                                        #   to contact if there is a problem

responce = stats.make_request(host="erikberg.com", sport=None, method="events",
                              id=None, format="json",
                              parameters={'sport': 'nba', 'date':'20130414'})

```

##Get teams
```python
stats = XMLStats(access_token='xxxxxxxxxxxxxxxxxxxxxxxxxxx',
                 email='some@email.com')
teams = stats.get_teams()
```

