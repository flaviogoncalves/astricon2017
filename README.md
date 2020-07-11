# Astricon 2017, comparing chan_sip versus pjsip

SIPP XML files and conf files for the presentation chan_sip versus han_pjsip

This files were created for the Astricon Presentation in 2017, it can be found at: https://www.youtube.com/watch?v=1HqoqjKbeIo

The Asterisk project improved a lot in the year after this presentation as shown at: https://www.youtube.com/watch?v=fhjtKT3BHhI, congratulations!

# Echo test with no media or authentication

Command Line

sipp -s 1000 ip_address:5060 -sn uac -i ip_address -d 1000

# Echo test with media

Command line

sipp -s 1000 ip_address:5060 -sf sipp_pcap.xml -i ip_address -d 90000


