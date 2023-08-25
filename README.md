# Huawei-E3372h-320-IP-Range-change
Method to change IP-Range of Huawei E3372h-320 LTE 4G Stick for use with proxies, bonding routers, belabox encoder, speedify etc.

<b>I do not take any responsibility for damaged devices following the use of this script! Do this on your own risk!</b>

If you want to use multiple Huawei 4G Sticks on one device you will get into problems because they all use 192.168.8.1 as IP by default.
While MiFi routers from Huawei let you change the IP address and its ranges the 4g USB Sticks don´t let you do this via the web UI.

There are some tools to change the IPs on github, but for me they didn´t work.
So I did some research and found a solution on https://mobileproxy.space/en/pages/configuring-the-e3372h-320-modem-to-work-with-mobile-proxies.html
I used this bookmark script to change the IP range of my branded Huawei E3372h-320 from 1&1 Internet (german ISP).
But since nobody in the world is able to read cyrillic letters I wanted to change the script into english so other people don´t have to translate cyrillic letters from Unicode to actual letters and afterwards translate it via google translator ;)


How to change IP:
1. Stick your device into your PC and let the web UI open itself.
2. create a bookmark by inserting the raw code of [script.txt](script.txt) of this repo into the URL line of the bookmark creation dialogue of your browser.
3. With the stick´s web ui opened click on the bookmark. You have to be in the tab or window of the web ui, because it directly interacts with the UI!
4. First it will ask for the current IP range. Most Huawei devices I know use 192.168.8.1 as the default IP. This is why '8' is pre filled in the prompt. So for default cases just press enter.
5. In the next step it will ask for the NEW IP address Range. If you type '100' in there, the device will afterwards be reachable by '192.168.100.1' for example. Just press enter afterwards and your device should automatically reinitialize and be reachable by the new IP after a few seconds.

<b> Update 25.08.2023: Works with E3372-325 (successor of E3372-320) too. 
thanks to @arakis86 :)
