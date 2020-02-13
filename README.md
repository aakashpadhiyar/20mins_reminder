# Eye Health
         the 20-20-20 rule

## Startup script on startup

		$ sudo nano /etc/systemd/system/startup.service

		  [Unit]
		  Description=Startup

		  [Service]
		  ExecStart=/usr/local/bin/the2020
		  [Install]
		  WantedBy=default.target


		$ sudo nano /usr/local/bin/startup.sh

		  #!/bin/bash

		  date > /root/report.txt
		  du -sh /home/ >> /root/report.txt

		$ sudo chmod 744 /usr/local/bin/startup.sh
		$ sudo chmod 664 /etc/systemd/system/startup.service
		$ systemctl daemon-reload
		$ systemctl enable startup.service

		# Test the script
		$ systemctl start startup.service
		$ cat /root/report.txt

		# Reboot
		$ sudo reboot

		# Change password for user ubuntu
		$ sudo passwd ubuntu

## SCRIPT
		./the202020

## audio
![](https://raw.githubusercontent.com/aakashpadhiyar/20mins_reminder/master/audio.mp3)		
# In every 20mins this file play a ringtone to alert you

www.github.com/aakashpadhiyar

Skype:      8afc3e69a745ee48

OR

Skype-link: https://join.skype.com/invite/eAkxgNXfjRHm

The 20-20-20 rule was designed by Californian optometrist Jeffrey Anshel as an easy reminder to take breaks and prevent eye strain, according to the Optometry Times.

When following the rule, a person takes a 20-second break from looking at a screen every 20 minutes. During the break, the person focuses on an object 20 feet away, which relaxes the eye muscles.

The following methods can help a person to put this rule into practice:

    Set an alarm for every 20 minutes while working, as a reminder to take a break.
    this an application developed to help people follow the 20-20-20 rule.
    Look out a window during the 20-second breaks. Judging a distance of 20 feet inside can be difficult, but focusing on a tree or lamppost across the street should work well.

Alternately, a person can benefit from closing their eyes for 20 seconds every 20 minutes. Also, remembering to blink can prevent dry eye by encouraging tear production.

Anyone who spends the day sitting should periodically get up and walk around, to prevent back and neck pains.

https://www.medicalnewstoday.com/articles/321536.php
