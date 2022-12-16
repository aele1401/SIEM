# Using Splunk

## The Need for Speed:

- Based on the report created, what is the approximate date and time of the attack?
	* Splunk query `source="server_speedtest.csv" | eval ratio = (UPLOAD_MEGABITS / DOWNLOAD_MEGABITS ) | table_time, IP_ADDRESS, DOWNLOAD_MEGABITS, UPLOAD_MEGABITS)`
- How long did it take your systems to recover?
	* System crash occurred 02/22/2020 at 23:30:00 hours and full system recovery at 02/23/2022 23:30:00 hours. Therefore, it took 24 hours for full system recovery.
	
	![Diagram](https://github.com/aele1401/SIEM/blob/main/Images/speedtest.PNG)

## Drawing the (base)line:

- When did the brute force attack occur?
	* Brute force attack occurred 05/02/2021 at 03:22:05AM AM. We know it occurred at this time because we have 25 intrusion attempts made to access the user account.
	
	![Diagram](https://github.com/aele1401/SIEM/blob/main/Images/bruteforce.PNG)

	

	



