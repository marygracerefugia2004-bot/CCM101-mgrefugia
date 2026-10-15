# Mission 8 Reflection

## 1. How does a host-based firewall protect a server even if the physical network perimeter is breached?

A host-based firewall protects a server by controlling the network traffic that reaches it. Even if the main network security is breached, the firewall can still block connections that are not allowed by its rules. This provides another layer of protection for the server.

## 2. Why is managing open network ports critical to reducing a server's attack surface?

Managing open ports is important because every unnecessary open port can give attackers another possible way to access the server. Allowing only the ports needed by the application reduces the attack surface and limits unnecessary network access.

## 3. In a real enterprise environment, why is it dangerous to leave a database port like 3306 for MySQL open to the public internet?

Leaving MySQL port 3306 open to the public internet is dangerous because attackers could attempt to guess passwords, exploit vulnerabilities, or access sensitive information. Database access should be restricted to trusted systems and authorized users instead of being available to everyone online.

## 4. How did completing this mission change your perspective on how easily a server can be compromised?

This mission helped me realize that an exposed server can become a target if it is not properly secured. I learned that security settings should be applied early and checked regularly. I also understood why SSH must be allowed before enabling a firewall to avoid blocking remote administration.

## 5. How does your GitHub portfolio currently look with eight completed missions?

My GitHub portfolio now contains eight cloud computing missions that show my progress in learning different cloud technologies. Each activity adds new knowledge and practical experience. I am becoming more confident in organizing files, documenting commands, and understanding server security. I still need more practice, but this mission helped me appreciate the importance of careful configuration and regular security checks.
