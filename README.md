# Sherlocks Tomes
Repository for BlueTeam Final Project


This repo contains files and information regarding our Blue Team Final project for Fullstack Academy.

There is a mini-challenge available called 'Sherlock's Tomes' to walk you through the various forensic techniques that we discuss in our video.


Challenge:

While you--Sherlock, were out on a solo case, Watson got bored and decided to play a video game on your computer. When he tried to download it, he noticed he had to free up some space. Watson located 6 files and decided that they seemed rather unimportant. He didn’t want Sherlock to find out, so he used an erasing program to delete one. After noticing how long that would take, he decided to just press the delete key on the remaining 5. He was then able to download the video game, which didn’t seem to work at all! Defeated, Watson put the computer back to sleep, and snuck out of your study.

When you got home, your computer was missing some important ‘tomes’ you need, as well as the fact that your system may be compromised!

“The game is afoot…” you whisper to yourself as you begin forensic analysis of what’s happened…

Files:
1. a .dd image of Sherlocks computer

  -md5 hash:

2. a .pcap file of network traffic taken from the incident

3. log file(s) containing information of CLI inputs or downloaded programs (journalctl.log[journalctl | tail -n100 | grep -r "/bin/rm" > journalctl.log] this command removes the evidence of removal.


									-this log file shows CLI sudo input as well as filenames of downloads
									-we must run 'wipe' and should consider altering date/time in log
									to match pcap if we have time




QUESTIONS:
1. What game did Watson download? - provide the full filename 

2. What IP Address and MAC Address did it come from?

3. Find/rebuild as many of the six tomes you can, and speculate as to why you can't find some.
	-leave hint file stating all 6 tomes' names.
	-have '_sudo wipe_' usage included in log file.

4. If Watson didn’t want the files recovered, what could he have done differently?

5. Sherlock’s computer seems like it may be compromised! What file do you think caused this? - provide the filename

6. What would be the most effective way to eliminate the threat from Sherlock's machine?

