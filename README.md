# wireshark_traffic_analysis
Task 5: Capture and Analyze Network Traffic Using Wireshark 
Objective: Capture live network packets and identify basic protocols and traffic types  Tools: Wireshark (free). 
Deliverables: A packet capture (.pcap) file and a short report of protocols identified.
🔧 Step 1: Install Wireshark
What to do:
1.	Go to https://www.wireshark.org/download.html.
2.	Download the installer based on your operating system (Windows/macOS/Linux).
 ![image](https://github.com/user-attachments/assets/d822c706-2f31-4952-ac60-f3d14a7368cb)

3.	Run the installer and follow the on-screen instructions.
4.	On Windows, during installation, allow WinPcap or Npcap to be installed — this is required to capture packets.
 ![image](https://github.com/user-attachments/assets/938321ee-42d8-43a6-8957-7a7eee5931e9)


Purpose:
Wireshark is a network protocol analyzer. Installing it lets you capture and view real-time network data.
________________________________________
🌐 Step 2: Start Capturing on Active Network Interface
What to do:
1.	Open Wireshark.
2.	On the main screen, you’ll see a list of available network interfaces.
 ![image](https://github.com/user-attachments/assets/2e16edbf-a4f5-469a-a8cc-784671143e92)

3.	Identify the active interface (e.g., Wi-Fi if you're on wireless, or Ethernet if wired).
4.	Double-click the active interface to start capturing packets.
 ![image](https://github.com/user-attachments/assets/62dc4123-5d50-4410-91e3-f3e073436e4a)

 Purpose:
Wireshark must listen to the correct interface to capture your actual internet traffic.
________________________________________
🌍 Step 3: Generate Traffic (Simulate Network Activity)
What to do:
1.	While Wireshark is capturing:
o	Open a browser and visit a few websites (e.g., http://example.com, https://google.com)
o	Open Command Prompt or Terminal and type: ping google.com
 ![image](https://github.com/user-attachments/assets/4b4fb094-3c66-4dde-b01c-a459f7efb940)

2.	You can also open apps like email clients or YouTube for more diverse traffic.
Purpose:
This creates visible, analyzable traffic in the capture (like HTTP, HTTPS, DNS, ICMP).
________________________________________
⏹ Step 4: Stop Capture After a Minute
What to do:
1.	Let the capture run for about 1 minute.
2.	Click the red square “Stop” button at the top toolbar in Wireshark.
 
Purpose:
You only need a small sample to analyze multiple protocols. A minute of traffic is plenty.
________________________________________
🔍 Step 5: Filter Captured Packets by Protocol
What to do:
Use the filter bar (just below the toolbar) to view specific protocol packets.
Try filtering with:
•	http – Shows HTTP requests/responses.
   ![image](https://github.com/user-attachments/assets/e59a5342-1502-4db8-96ed-3c75ded57784)
   
•	dns – Shows domain name queries and replies.
  ![image](https://github.com/user-attachments/assets/941066ae-2ccb-429b-b022-f520955c23a5)
             
•	icmp – Shows ping traffic.
  ![image](https://github.com/user-attachments/assets/181ec34f-ae01-4221-baa2-0e4a3aec5ac2)

•	tcp – Shows all TCP traffic.
 ![image](https://github.com/user-attachments/assets/45bba063-5cd6-40da-9024-f301ef0d1574)

•	tls – Shows encrypted HTTPS traffic.
 ![image](https://github.com/user-attachments/assets/5404eaca-7c1b-4a69-ac0a-5a5796020dda)

Why:
Filtering helps you isolate and study specific types of traffic without being overwhelmed by other data.
________________________________________
🔎 Step 6: Identify At Least 3 Different Protocols
What to do:
Look at packet details and note:
•	The protocol name
•	What it's used for
•	Example packet contents
Example:
1.	DNS – Resolves domain names to IPs.
o	Filter: dns
o	Look for queries like A google.com
2.	HTTP – Web browsing (unencrypted).
o	Filter: http
o	Look for GET/POST requests
3.	ICMP – Used for ping.
o	Filter: icmp
o	Shows echo requests/replies
Why:
Understanding common protocols is essential for network analysis.
________________________________________
💾 Step 7: Export the Capture as a .pcap File
What to do:
1.	Go to File > Save As.
2.	Choose a location and name, e.g., network_traffic_analysis.pcap.
3.	Make sure the file format is set to Wireshark/tcpdump/... - pcap.
4.	Click Save.
      ![image](https://github.com/user-attachments/assets/cefeb52b-c3c2-4bad-ab2b-d51879d20d10)

Open file to capture and analyse network traffic using wireshark
Conclusion: 
Capturing and analyzing network traffic with Wireshark provides valuable insight into how data moves across a network. Through this hands-on activity, we were able to observe real-time packet exchanges, identify multiple network protocols (such as DNS, HTTP, TCP, and ICMP), and understand how devices communicate over the internet.
This exercise enhanced our understanding of:
•	Network layers and protocol functions
•	How requests (like browsing a website or pinging a server) generate specific traffic
•	The structure and content of packets in transit
By filtering and examining captured data, we developed fundamental skills in network troubleshooting, security monitoring, and protocol analysis — all of which are essential for anyone pursuing networking, cybersecurity, or IT.
Wireshark proves to be a powerful and accessible tool for visualizing network behavior and gaining a deeper awareness of how the internet works under the hood.

