# Protecting VSI from Future Attacks

## Windows Server Attack

- ***Several users were impacted during the attack on March 25th.***
- ***Based on the attack signatures, what mitigations would you recommend to protect each user account? Provide global mitigations that the whole company can use and individual mitigations that are specific to each user.***
	* Implement account policies and restrictions to user accounts.
	* Only allow connections from trusted sources or only accept domestic connections filtering out any foreign connections.
- ***VSI has insider information that JobeCorp attempted to target users by sending "Bad Logins" to lock out users.***
- ***What sort of mitigation could you use to protect against this?***
	* To proect users from getting completely locked out, some mitigation strategies are:
		- Utilize multi-factor authentication (MFA).
		- Notify users that, "Several login attempts were made, and the account has been locked. Contact support or reset password" to unlock the account.
		- Set time constraints on how long user accounts are locked. (Account locked for 1 hour)

## Apache Web Server Attack

- ***Based on the geopgraphic map, recommend a firewall rule than the Network Team should implement.***
- ***Provide a simple description of the rule in plain english.***
	* Since most of the traffic is coming from outside of the United States, a rule can be created to block all incoming foreign traffic.

	![Diagram](https://github.com/aele1401/SIEM/blob/main/Images/traffic.png)

- ***VSI has insider information that JobeCorp will launch the same web server attack, but use a different IP each time in order to avoid being stopped by the rule you just created.***
- ***What other rules can you create to protect VSI from attacks against your web server?***
	* Additional rules that can be created to circumvent these attacks are:
		- A special rule can be created which can block all incoming traffic with bytes over the 5000 threshold.
		- Consult and specify server and protection settings.
