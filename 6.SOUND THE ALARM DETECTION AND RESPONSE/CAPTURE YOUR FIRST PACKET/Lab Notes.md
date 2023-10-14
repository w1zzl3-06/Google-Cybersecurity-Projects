sudo ifconfig

Identifies the interfaces that are available.


sudo tcpdump -D

Identifies the interface options available for packet capture


sudo tcpdump -i eth0 -v -c5

This command will run tcpdump with the following options:
	•	-i eth0: Capture data specifically from the eth0 interface.
	•	-v: Display detailed packet data.
	•	-c5: Capture 5 packets of data.


Filters live network packet data from the eth0 interface


sudo tcpdump -i eth0 -nn -c9 port 80 -w capture.pcap &

Capture packet data into a file called capture.pcap

This command will run tcpdump in the background with the following options:
	•	-i eth0: Capture data from the eth0 interface.
	•	-nn: Do not attempt to resolve IP addresses or ports to names.This is best practice from a security perspective, as the lookup data may not be valid. It also prevents malicious actors from being alerted to an investigation.
	•	-c9: Capture 9 packets of data and then exit.
	•	port 80: Filter only port 80 traffic. This is the default HTTP port.
	•	-w capture.pcap: Save the captured data to the named file.
	•	&: This is an instruction to the Bash shell to run the command in the background.

curl opensource.google.com

Use curl to generate some HTTP (port 80) traffic

ls -l capture.pcap

Verifies that packet data has been captured

sudo tcpdump -nn -r capture.pcap -v

Filters the packet header data from the capture.pcap capture file

This command will run tcpdump with the following options:
	•	-nn: Disable port and protocol name lookup.
	•	-r: Read capture data from the named file.
	•	-v: Display detailed packet data.

*You must specify the -nn switch again here, as you want to make sure tcpdump does not perform name lookups of either IP addresses or ports, since this can alert threat actors.

sudo tcpdump -nn -r capture.pcap -X

This command will run tcpdump with the following options:
	•	-nn: Disable port and protocol name lookup.
	•	-r: Read capture data from the named file.
	•	-X: Display the hexadecimal and ASCII output format packet data. Security analysts can analyze hexadecimal and ASCII output to detect patterns or anomalies during malware analysis or forensic analysis.

Filters the extended packet data from the capture.pcap capture file


