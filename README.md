# Nicehash Notifier
Welcome to the NicehashNotifier GitHub Repository.<br />
Now, this app isn't anything too special, just a neat little program to send you email notifications when your Nicehash miner reaches your user defined milestones.<br />
<br />
Requirements:<br />
* An email address to send from (That you know the SMTP Server and Port for)
* An email address to send to
* An active Nicehash Miner
* Basic knowledge of editing a config file

# Editing the config
```
{
	"miner_info": [{
		"address": "",
		"isnicehashwallet": "yes"
	}],
	"goals": [{
		"bitcoin": "0.001",
		"gbp": "100.00",
		"usd": "100.00",
		"eur": "100.00"
	}],
	"notifications": [{
		"recipient_email_address": "",
		"sender_email_address": "",
		"smtp_server": "smtp.gmail.com",
		"smtp_port": "465"
	}],
	"alertincrements": [{
		"bitcoin": "0.01",
		"gbp": "10.00",
		"usd": "10.00",
		"eur": "10.00"
	}],
	"enabledalerts": [{
		"bitcoin": "true",
		"gbp": "true",
		"usd": "true",
		"eur": "true",
		"incremental": "true"
	}],
	"applicationsettings": [{
		"update_frequency": "60",
		"show_btc_rates": "true",
		"show_goal_progress": "true",
		"show_balance_change": "true"
	}]
}
```
Key | Value
------------- | -------------
miner_info > address  | The Address of your Nicehash Miner
miner_info > address  | Whether or not your Nicehash Miner is mining to a Nicehash Wallet
goals > bitcoin | Bitcoin goal
goals > gbp | GBP (£) Goal
goals > usd | USD ($) Goal
goals > eur | EUR (€) Goal
notifications > recipient_email_address | The email address to send the notifications to
notifications > sender_email_address | The email address from which the notifications will be sent
notifications > smtp_server | The SMTP server of the sending email address
notifications > smtp_port | The SMTP port of the sending email address
alertincrements | THIS WHOLE SECTION IS IN THE WORKS, YOU CAN IGNORE FOR NOW
enabledalerts > bitcoin | Enable/Disable Bitcoin Notifications
enabledalerts > gbp | Enable/Disable GBP Notifications
enabledalerts > usd | Enable/Disable USD Notifications
enabledalerts > eur | Enable/Disable EUR Notifications
applicationsettings > update_frequency | How often your balances/rates are updated in seconds (min 60)
applicationsettings > show_btc_rates | With this enabled, the application will output and updated Bitcoin Rate to GBP, USD & EUR (NOT YET IMPLEMENTED)
applicationsettings > show_goal_progress | With this enabled, the progress to your balance goals will be displayed alongside your balances
applicationsettings > show_balance_change | With this enabled, the change in balance since the last update will be displayed alongside your balances


## Upcoming Features
* Incremental Alerts, once initial goal is reached
* Payout Alerts, based on whether or not you have a Nicehash Wallet, you will get a notification when you surpass the payout threshold.
* Currently the application only supports SMTP SSL connections for email, working on allowing more.
* Better error handling, a lot of things just make it cry and crash!
* Then, in the distant future, making it UI Based.

### Donation Addresses
* BTC: 17gbJUL2Mi9McuM7J3FBW9ddyYyT6hLpX9
* LTC: LWtgC4HzMwmdDJTHYVRKhAgRbxXvmHeAyv

### Credits
Bitcoin values supplied by [CoinDesk](https://www.coindesk.com/) <br />
Uses [NiceHash](https://www.nicehash.com/) API
