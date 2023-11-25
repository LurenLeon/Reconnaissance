# Reconnaissance

# Learning Objectives

- Learn about reconnaissance and penetration testing tools (Nmap, Wireshark, and Nessus/Rapid7 Vulnerability scanners).
- Learn how to discover what’s on your network and identify vulnerable services/hosts.
- Learn about traffic analysis and TCP/IP protocols.

Part of your responsibility for this assignment is to learn how to work with new security tools. This is an important exercise because, as a cybersecurity specialist in any position, you must be able to put your theoretical understanding of security, network, and system concepts to use to solve real-world problems. To do this, you must learn how to work with new tools that are essentially built on the same theoretical concepts you've learned in class.

## Submission Guidelines

Please submit a PDF file that describes your detailed steps, results, and answers to the following questions.

## Rubrics for Grading

### Part 1: Port Scanning to Map a Network (35% total)

- Complete scanning including the list of IP addresses of all machines in the network, OS and version, open ports, services running on ports and versions (35%)
- Fairly incomplete report, missing some of the information (max 20%)
- Incomplete report, missing most or all of the important information (0%)

### Part 2: Vulnerability Scanning (35% total)

- Complete vulnerability scanning, including a list of the top 5 discovered vulnerabilities, and analysis of vulnerabilities (CVE information about each) (30%)
- Fairly incomplete report, missing discovered vulnerabilities, or analysis of vulnerabilities (max 20%)
- Incomplete report, missing most or all of the important information (0%)

### Part 3: Traffic Analysis with Wireshark (30% total)

- Complete analysis, including answers to all questions (30%)
- Incomplete analysis, missing answers to some of the questions, 5% deducted for each missing answer.
- Incomplete analysis, missing most or all of the important information (0%)

# Assignment Description

## Part 1: Port Scanning to Map a Network (35 points)

Use Nmap/Zenmap to scan your own home network. Ethical practice: please do not scan somebody else’s network; this is unethical and could get you in trouble.

## Part 2: Vulnerability Scanning (35 points)

Use Nessus or Rapid7 Vulnerability scanners to scan one of these machines remotely (or locally, but remotely is preferred). Go through the generated report by the vulnerability scanner and list your top 5 vulnerabilities that you discovered.

## Part 3: Traffic Analysis with Wireshark (30 Points)

Run Wireshark and start capturing packets on your own main NIC. Then, open the browser and visit a website like Wikipedia.com. Wait for 30 seconds and stop the capture.

Use Wireshark filters to answer the following questions. Anonymize IP and MAC addresses in your responses (replace some letters from the middle with space).

### 3.1. Define a Display filter that finds the ARP queries and ARP responses.

Narrow down the filter so that only those ARP packets are shown that were necessary for opening your chosen webpage (the rest of the captured ARP packets that were exchanged between the nodes of LAN should be left out of the list).

### 3.2. What is the transport layer protocol used in the DNS query packet? What is the decimal number in the network layer header that identifies this protocol?

### 3.3. Define a display filter that finds the DNS queries and DNS responses.

Narrow down the filter so that only those DNS packets are shown that were necessary for opening your chosen webpage (the captured DNS packets that were related to other applications/clients in your computer should be left out of the list).

### 3.4. Using the filters created in the previous steps, list all the ARP query/response pairs and DNS query/response pairs necessary for opening your chosen webpage.

For each ARP query/response pair and DNS query/response pair, explain the following (you can group the queries and responses to avoid repetitions in your explanations):

- What information was asked for (show the relevant information in the query)
- Who was it asked from (what was the MAC address and IP address of it)
- Who answered (what was the MAC address and IP address of it)
- What information was in the answer (show the relevant information in the response)
- Justify why the query was made.
