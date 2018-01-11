# Nicehash Notifier
Howdy, welcome to the NicehashNotifier GitHub Repository.<br />
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
		"address": "",						<-- Your Nicehash Miner Address
		"isnicehashwallet": "no"			<-- Whether or not you're mining to a Nicehash wallet
	}],
	"goals": [{
		"bitcoin": "0.01",					<-- Your Bitcoin Goal
		"gbp": "100.00",					<-- Your GBP Goal (£)
		"usd": "100.00",					<-- Your USD Goal ($)
		"eur": "100.00"						<-- Your EUR Goal (€)
	}],
	"notifications": [{
		"recipient_email_address": "",		<-- The email to send the notifications to
		"sender_email_address": "",			<-- The email of the sender
        "smtp_server": "smtp.gmail.com",	<-- The SMTP Server of the Sending Email Address
        "smtp_port": "465"					<-- The SMTP Port of the Sending Email Address
	}],
	"alertincrements": [{
		"bitcoin": "0.01",					<-- Currently a work in progress, you can ignore this for now
		"gbp": "10.00",						<-- Currently a work in progress, you can ignore this for now
		"usd": "10.00",						<-- Currently a work in progress, you can ignore this for now
		"eur": "10.00"						<-- Currently a work in progress, you can ignore this for now
	}],
	"enabledalerts": [{
		"bitcoin": "true",					<-- Enable/Disable alerts for Bitcoin
		"gbp": "true",						<-- Enable/Disable alerts for GBP
		"usd": "true",						<-- Enable/Disable alerts for USD
		"eur": "true"						<-- Enable/Disable alerts for EUR
	}]
}
```

## Credits
Bitcoin values supplied by [CoinDesk](https://www.coindesk.com/)
