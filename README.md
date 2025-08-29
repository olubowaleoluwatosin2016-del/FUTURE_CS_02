
SOC Incident Response Report.

1. Executive Summary
On 2025-07-03-2025-07-04, multiple failed login attempts and malware detection alerts were observed on corporate systems. Immediate investigation confirmed a brute-force attack on the server, a trojan and ransomware infection and also connection attempts on four endpoints.

2. Incident Details
Incident ID
Date & Time Detected
SIEM Tool Used
Detection Method
Systems/Accounts Affected
SOC-20250703-01
2025_07_0304:47:14 04:23:14
   Splunk
Splunk alert – Multiple failed logins
        1
SOC-20250703-02
2025_07_0307:45:14
   Splunk
Antivirus alert – Trojan detected
    1
SOC-20250703-03
2025_07_0309:10:14
   Splunk
Antivirus alert – Ransomware Behaviour
         1
SOC-20250703-04
2025_07_0307:44:14
  Splunk
Splunk alert connection attempt
         1












3.Timeline
Time (UTC)


Incident ID


Event Description
04:47
SOC-20250703-01
Splunk  alert triggered for 4 failed logins from IP 10:0.0.5
04:49

SOC-20250703-01
Analyst began investigation in Splunk dashboard
04:51

SOC-20250703-01
Confirmed brute-force pattern
04:55

SOC-20250703-01
Incident documented in response report



Time (UTC)
Incident ID
Event Description
07:44
SOC-20250703-02
Splunk  alert failed  connection attempt  
07:46

SOC-20250703-02
Analyst began investigation in Splunk dashboard
07:48

SOC-20250703-02
Confirmed brute-force pattern
07:52

SOC-20250703-02
Incident documented in response report


Time (UTC)
Incident ID
Event Description
07:45
SOC-20250703-02
Splunk  alert Trojan malware detected
07:47

SOC-20250703-02
Analyst began investigation in Splunk dashboard
07:49

SOC-20250703-02
Confirmed trojan malware attempt
07:53

SOC-20250703-02
Incident documented in response report


Time (UTC)
Incident ID
Event Description
09:10
SOC-20250703-02
Splunk  alert Ransomware  behaviour
09:12

SOC-20250703-02
Analyst began investigation in Splunk dashboard
09:14

SOC-20250703-02
Confirmed ransomware pattern
09:18

SOC-20250703-02
Incident documented in response report




4. Severity Classification
Alert ID
Incident ID
Description
Severity (High/Medium/Low)
Reason
A-01
SOC-20250703-01
8 failed logins from IP:
10.0.0.5 ,  172.16.0.3
High
Brute-force attack
A-02
SOC-20250703-002
Malware detected on PC
Critical
Trojan infection found
A-03
SOC-20250703-03
Malware detected on PC
Critical
Ransomware Behaviour
A-04
SOC-20250703-04
Failed connection attempt
Medium
Brute-force attack



5. Impact Assessment
Potential data exposure: 
 a] No confirmed data loss, but HR employee credentials were  exposed.
 b] Malware could have compromised Sensitive files which could be damaged/Lost.


Business impact: 
a] Could have caused reputational damage if client data was leaked.
b] No operational impact — incident contained before access was granted.

Duration of threat presence: 
a] Brute-force attempts lasted for 5 minutes before IP was blocked




6. Remediation & Next Steps
Containment: 
a] Block IP, Lock affected accounts, Disconnect affected system from the network.


Eradication: 
a] Remove trojan, update antivirus software.


Recovery: 
a] Recover all ransomware systems and update system from backup.


Prevention: 
a] Install Intrusion detection system and Intrusion prevention system.
b] Apply stricter firewall rules.



7. Attachments
SIEM screenshots (dashboard + alert details) 
 Alert details:  
Dashboard: 

  
    












Incident Communication Email 
Subject: Incident Report – SOC_Task2_Sample_Logs
To: SOC team
 Date: 07-03-2025

Dear SOC team,
This is to formally report a security incident detected on 07-03-2025 12:00 am - 12:00pm involving: unauthorized login attempts, ransomware behavior, connection attempts and Trojan detection.
Summary of Incident:
 On 07-03-2025 12:00 am - 12:00pm, the splunk alert tool flagged an anomaly of multiple failed login attempts from an unfamiliar IP address, connection attempts for different IP addresses, trojan attempt and ransomware attack. Investigation confirmed compromised account, infected endpoint, attempted data exfiltration.
Incident Details:
Incident ID: SOC-20250703-01, SOC-20250703-02, SOC-20250703-03, SOC-20250703-04


Category: failed login, trojan detection, ransomware behaviour, connection attempts


Severity Level: High, Critical, Medium


Affected Systems/Accounts: 4


Detection Method: splunk alert


Impact Assessment:
Business Impact: minor disruption to user access, risk to customer data.


Data Compromise: No sensitive Data was Leaked.




Actions Taken So Far:
Isolated affected systems.


Blocked malicious IP addresses.


Reset compromised credentials.


Applied security patches/updates.


Next Steps:
Continuous monitoring for related activity.


Conduct root cause analysis.


Please advise on any additional actions or escalation needed.
Regards,
 Oluwatosin Ruth olubowale
 Cybersecurity Intern.
 ruthmorenikejiolubowale@gmail.com

