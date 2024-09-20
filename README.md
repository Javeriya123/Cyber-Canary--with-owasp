Network canaries act as early warning systems by luring attackers to interact with decoy resources, such as files or services, which are closely monitored by Administrators who are notified of possible intrusions when these canary assets are accessed or altered, as alerts are raised. The term cyber canary describes a cybersecurity idea that was influenced by the old method of detecting hazardous gas carbon monoxide in coal mines by carrying a canary bird the death of the canary alerted the miners to a high level of gas and miners would leave the place to protect themselves from the hazardous gas.

There is a challenge in mapping the attacks with real-time vulnerabilities so that the attack can be identified at an earlier stage to protect the network. The flexible network configuration for canaries and map it with OWASP vulnerabilities in real time to identify threats such as security misconfiguration, Injection, and Broken Access Control. To alert any interaction with the vulnerable machines a central server is created to monitor any activity more closely. Hence integrating the network of canary machines with rsyslog significantly enhances real-time threat detection.

To mimic the OWASP Top 10 vulnerabilities, a network of susceptible Ubuntu Virtual Machine (VM) running FTP, MySQL, and LDAP services has been established. Controls selected as of 2021 are Broken Access Control (A01), Injection (A03), and Security Misconfiguration (A05). These systems are vulnerable to attacks due to data manipulation, unauthorized access, and misconfigurations. The ability to generate logs when any action takes place inside the network has been set up to have centralized logs using the rsyslog utility where the logs from each vulnerable machine are accumulated and available for detection.

The vulnerable machines are successfully placed in the network as canaries; any interaction with these canary machines results in alerting the centralized server. Any interaction or modification is seen through the logs. The segregation of logs done at the centralized server is accurate and helps in analyzing the logs concerning the vulnerable machine.