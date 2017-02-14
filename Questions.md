#Questions

1. The ticket forwarding sent every time a ticket is issued or only when stop.

I think that in GSM /GPRS its sent every time a ticket is issued.

My guess would be every time a ticket is issued.

300 buses in Madurai => Scalable or not? One bus every few seconds I'm sending a couple of kbs of data - all over tn - server will be receiving simultaneous load requests....

Similarly, Server load problem?

Or Network bandwith - traffic  problem? I don't think so.. what's your take?

2. The on-board computer is going to have to balance 3 works:

State my requirements - do you think that theses requirements can be balanced -with the individual shields??

1. Get GPS info every 10 secs
2. Send the GPS info to server as soon as received. If the GSM/GPRS network is not available, then store the data in memory - accumulate it. (Bad situation) When the GSM network becomes available again, send the accumulated data to the server.

3. GPS receiver on top of the bus or if connected to battery - will the GPS be able to receive signals/?

(Depending on the above question decide whether battery powwered or vehicle powered...)

i.e. WHERE to install the gps?


4. Once I've chosen where to install the GPS - what about the Bluetooth Low Energy the ETM should be able to send the data via Bluetooth 4.2 to the on-board computer with Bluetooth 4.2 interface shield. 

Question is: If On-board computer is installed on top of the bus or under the bus, or near wheel wall, can the signal from the bluetooth 4.2 reach the on-board computer?

Since, wi-fi & bluetooth 4.2 use the same frequency fo rtransmission - If someone is using wi-fi on their phone will those signals interfere with my bluetooth signal?
