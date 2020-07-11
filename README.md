# astricon2017

SIPP XML files and conf files for the presentation chan_sip versus han_pjsip

This files were created for the Astricon Presentation in 2017, it can be found at: https://www.youtube.com/watch?v=1HqoqjKbeIo

# Echo test with no media or authentication

Command Line

sipp -s 1000 10.8.1.46:5060 -sn uac -i 10.8.1.46 -d 1000

extensions.conf

[from-internal]
exten=>1000,1,Answer()
exten=>1000,n,Echo()
exten=>1000,n,Hangup()
exten=9000,1,Answer();
exten=9000,n,MusicOnHold()

# Echo test with media

Command line

sipp -s 1000 10.8.1.46:5060 -sf sipp_pcap.xml -i 10.8.1.46 -d 90000


