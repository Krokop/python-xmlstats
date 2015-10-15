# python-xmlstats
python module for https://erikberg.com/api

#Install
```bash
pip3 install python-xmlstats
```
#Use
```python
from xmlstats import XMLStats

stats = XMLStats(access_token='xxxxxxxxxxxxxxxxxxxxxxxxxxx',
                 user_agent='xxxxxxxx') # Replace with your bot name and email/website 
                                        #   to contact if there is a problem
                                        #   e.g., "mybot/0.1 (https://erikberg.com/)"

responce = stats.make_request(host="erikberg.com", sport=None, method="events",
                              id=None, format="json",
                              parameters={'sport': 'nba', 'date':'20130414'})

```
