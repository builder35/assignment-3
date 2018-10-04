Intended OS: Windows

usage: scanner.py [-h] [-ip_addr [I]] [-po [PO]] [-tcp] [-udp] [-trace] [-ps]

Penetration testing port/ip scanner

optional arguments:
  -h, --help            show this help message and exit
  -ip_addr [I]          ip_address(es) to scan: format can be a singl address
                        or comma seperated
  -po [PO]              port(s) to scan: format can be [p, 1 - n , comma
                        seperated]
  -tcp, --tcp_scan      perform a tcp port(s) scan
  -udp, --udp_scan      perform a udp port(s) scan
  -trace, --trace_route
                        perform a traceroute
  -ps, --ping_sweep     perform a ping rquest/sweep

Additional usage information: 

All of flags can be used at once exccept for --help it will override the others

Only two flags require user input ( ip_addr and -po ) 

Ip addresses can be comma seperated, CIDR, or just a single adress
	DONT MIX FORMATS

Ports can be a single port, comma seperated , or '-' seperated
	DONT MIX FORMATS

YOU MUST BE PHYSICALLY CONNECTED TO THE NETWORK TO DO A UDP SCAN
I was unable to figure out why this but was unable to 
get the problem solved.