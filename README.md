# Reminder Bot for Discord 🕑
This is a custom Reminder Discord bot

## Install Directly on a local computer

- Create a [Bot account](https://discordpy.readthedocs.io/en/stable/discord.html) and invite the Bot to a Discord server

- Add `main.py` and `keep_alive.py` to a new repository on [Replit](https://replit.com/)

- Replace `TOKEN` with the Discord Bot token

## Replit

Run the following in the bash shell:

`pip install discord`

`pip install python-dateutil`

`pip install buttons`

`pip install aioschedule`

`pip install tzlocal`

`pip install pytz`

- Then run `main.py`, this should generate a URL `https://reminderbot.winniiew.repl.co/` that can then be used in [UptimeRobot](https://uptimerobot.com/) to host the Discord bot.

### Uptime Robot
1. Click `+ Add New Monitor`
2. Select `HTTP(s)` under `Monitor Types`
3. Paste the generated URL
4. Change the monitoring interval to 5 minutes

<p align="center">
<img width="500" alt="reminder2" src="https://user-images.githubusercontent.com/86391366/172505916-782aff26-2fb2-4c0a-abef-a5dd9e0767e1.PNG">
<p>

Change the [timezone](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) by following the format below

```python
tzinfos = {"<COUNTRY_CODE>": tz.gettz("<TZ_NAME>")}

dt = parser.parse(f"{dt} <COUNTRY_CODE>", tzinfos=tzinfos)
```
  
`<COUNTRY_CODE>` with the desired country code 
 
`<TZ_NAME>` with the timezone database name matching the country code
  
  
**Example**
```python
tzinfos = {"US": tz.gettz("America/Los_Angeles")}

dt = parser.parse(f"{dt} US", tzinfos=tzinfos)
```
  
## Invite Bot to join server
https://discord.com/api/oauth2/authorize?client_id=983852362269609984&permissions=534723897408&scope=bot

## Commands

`/remindme 15m Laundry`

`/remindme 16:30:00 Feed the dog`
  
 ### Units Supported
  
  `s` `second` `seconds` 
 
  `m` `minute` `minutes`
  
  `h` `hour` `hours`
  
  `d` `day` `days`
  
  `w` `week` `weeks`
  
  `mo` `month` `months`
  
  `y` `year` `years`




