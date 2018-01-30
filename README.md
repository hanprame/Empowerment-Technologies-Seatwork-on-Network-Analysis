# Empowerment-Technologies-Seatwork-on-Network-Analysis

ipconfig / ifconfig
Exercise:
Run ipconfig on your machine. What is your machine's IP address and subnet mask? Compare it with your seatmate.

My Machines IP Address: 192.168.0.35
Ping Latency:
          Packets: sent=4, received = 0, Lost = 4(100% Lost),

ping
Exercise:
Get your seatmate's IP address and ping it. What was the ping latency?

My seatmates IP Adress: 192.168.0.35
Ping Latency: Packets: sent = 4, received = 0, Lost = 4(100% Lost),

ping the following web sites:

www.telkom.co.za (South African telecommunications company)
www.singtel.sg (a Singaporean telecommunications company)
www.pldt.com.ph (a Philippine telecommunications company)
www.att.com (a US telecommunications company)

Telkom
      Ping statistics for 165.143.151.45:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 491ms, Maximum = 492ms, Average = 491ms
    
Singtel
       Ping statistics for 203.127.23.18:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 386ms, Maximum = 399ms, Average = 394ms

PLDT
      Ping statistics for 210.14.4.124:
    Packets: Sent = 4, Received = 0, Lost = 4 (100% loss),
    
Akamai Edge
      Ping statistics for 184.84.55.130:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 81ms, Maximum = 82ms, Average = 81ms
    
tracert / traceroute
Exercise:
Do a traceroute for each of the four websites you pinged in the previous exercise. Which has the most, and which has the least number 
of hops? For each traceroute, identify the bottleneck (takes the longest time) hop.

Descending order speed rank

1.PLDT - Average : 26ms(our broadband connection speed)
2.Akamai Edge - Average : 81ms
3.Singtel - Average :394ms
4.Telkam - Average :491ms

whois
Exercise:
For each of the hops in the traceroute output to www.singtel.sg, run a whois. Determine the location (country) of each IP address 
in the hop. Do the same analysis for the traceroute output to www.att.com. Based on your analysis, explain which network connection 
is faster, and why.

Singtel
      country: Singapore
Akamai Edge
      country: United States
      
netstat
Exercise:
Run netstat on your machine. You might need to press Ctrl-C to stop netstat.

From the netstat output, what are the remote machines that you're connecting to?


C:\Users\Hanna>netstat

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    192.168.2.104:49157    95.183.2.30:http       CLOSE_WAIT
  TCP    192.168.2.104:49159    68.232.45.253:http     CLOSE_WAIT
  TCP    192.168.2.104:49173    ec2-54-169-9-185:http  ESTABLISHED
  TCP    192.168.2.104:49226    ec2-52-1-89-36:https   ESTABLISHED
  TCP    192.168.2.104:49244    ec2-52-193-29-219:https  ESTABLISHED
  TCP    192.168.2.104:49254    ec2-34-235-239-92:https  ESTABLISHED
  TCP    192.168.2.104:49320    hkg07s02-in-f10:https  FIN_WAIT_2
  TCP    192.168.2.104:49360    lb-192-30-255-113-sea:https  FIN_WAIT_2
  TCP    192.168.2.104:49362    lb-192-30-255-117-sea:https  FIN_WAIT_2
  TCP    192.168.2.104:49384    hkg12s11-in-f10:https  FIN_WAIT_2
  TCP    192.168.2.104:49499    61:http                ESTABLISHED
  TCP    192.168.2.104:49602    ec2-52-59-36-167:https  CLOSE_WAIT
  TCP    192.168.2.104:49631    ec2-52-72-239-208:https  ESTABLISHED
  TCP    192.168.2.104:49807    tj-in-f188:5228        ESTABLISHED
  TCP    192.168.2.104:49905    lb-192-30-253-125-iad:https  ESTABLISHED
  TCP    192.168.2.104:49995    106.38.184.136:http    TIME_WAIT
  TCP    192.168.2.104:49996    ec2-34-198-0-91:https  ESTABLISHED
  TCP    192.168.2.104:49997    106.38.184.136:http    TIME_WAIT

C:\Users\Hanna>



remote machines that I'm connecting to:

TCP    192.168.2.104:49173    ec2-54-169-9-185:http
TCP    192.168.2.104:49226    ec2-52-1-89-36:https
TCP    192.168.2.104:49244    ec2-52-193-29-219:https
TCP    192.168.2.104:49254    ec2-34-235-239-92:https
TCP    192.168.2.104:49499    61:http
TCP    192.168.2.104:49631    ec2-52-72-239-208:https
TCP    192.168.2.104:49807    tj-in-f188:5228
TCP    192.168.2.104:49905    lb-192-30-253-125-iad:https
TCP    192.168.2.104:49996    ec2-34-198-0-91:https

Established states
