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
`
{ <br />
	"miner_info": [{
		"address": "",
		"isnicehashwallet": "no"
	}],
	"goals": [{
		"bitcoin": "0.01",
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
		"eur": "true"
	}]
}
`
