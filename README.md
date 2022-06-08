This is a custom Reminder Discord bot

Possible commands:
`/remindme 15m Laundry`

`/remindme 16:30:00 Feed the dog`

Install libraries in bash shell:

`pip install discord`

`pip install python-dateutil`

`pip install buttons`

`pip install aioschedule`

`pip install tzlocal`

`pip install pytz`

Change the timezone by altering these lines. List of timezones can be found here: https://en.wikipedia.org/wiki/List_of_tz_database_time_zones

`tzinfos = {"US": tz.gettz("America/Los_Angeles")}`

`dt = parser.parse(f"{dt} US", tzinfos=tzinfos)`

Then run `main.py`, this should generate a URL `https://reminderbot.winniiew.repl.co/` that can then be used in https://uptimerobot.com/ to host the Discord bot.

Uptime Robot:
1. Click `+ Add New Monitor`
2. Select `HTTP(s)` under `Monitor Types`
3. Paste the generated URL
4. Change the monitoring interval to 5 minutes

<img width="441" alt="reminder2" src="https://user-images.githubusercontent.com/86391366/172505916-782aff26-2fb2-4c0a-abef-a5dd9e0767e1.PNG">

Result:

<img width="250" alt="remind" src="https://user-images.githubusercontent.com/86391366/172505493-59d4c369-7a60-4e29-933e-da677144e6d0.PNG">
