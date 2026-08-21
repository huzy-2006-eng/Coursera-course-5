Vulnerablity assessment - The internal review process of an organization's security systems.
Process -
1. **Identification** -
Here,scanning tools and manual testing is used to find vlnerabilities.
2. **Vulnerability analysis** -
Each of the vulnerabilities that were identified are tested.
3. **Risk assessment** -
a score is assigned to each vulnerability. The score is given based on two factors ;
    1. How severe the impact would be if the vulnerability is exploited
    2. The likelihood of this happening.
4. **Remediation** -
Depends on the risk assessment score assigned.

# Vulnerability Scanner:
A vulnerability scanner is software that automatically compares known vlnerabilities and exposures against the technologies on the network. 
In general, these tools can scan systems to find misconfigurations or programming flaws.
Scanning tools are used to analyze each of the attack surfaces:
1. Perimeter layer, like authentication systems that validate user access

2. Network layer, which is made up of technologies like network firewalls and others

3. Endpoint layer, which describes devices on a network, like laptops, desktops, or servers

4. Application layer, which involves the software that users interact with

5. Data layer, Which includes any information that's stored, in transit,or in use.

When a scan of any layer begins, the scanning tool compares the findings against databases of security threats. At the end of the scan, the tool flags any vulnerabilities that it finds and adds them to its reference database. Each scan adds more information to the database, helping the tool be more accurate in its analysis.

# Performing scans:
Vulnerability scanners are meant to be non-intrusive. Meaning, they don't break or take advantage  of a system like an attacker would. Instead, they simply scan a surface and alert u to any potentially unlocked doors in your systems.

# Types of Scans:
1. **External scans** test the perimeter layer outside of the internal network. They analyze outward facing systems,like websites and firewalls. These kinds of scans can uncover vulnerable things like vulnerable network ports or servers.
2. **Internal scans** start from the opposite end by examining an organization's internal systems. For example, this type of scan might analyze application software for weakness in how it handles user input.

3. **Authenticated scans** might test a system by logging in with a real user account or even with an admin acccount. These service accounts are used to check for vulnerabilities, like broken access controls.

4. **Unauthenticated scans** simulate external threat actors that do not have access to your business resources.
For example, a scan might analyze file shares within the organization that are used to huse-internal only.  Unauthenticated users should receive "access denied" results if they tried opening these files. However, a vulnerability would be identified if you were able to access a file.

5. **Limited scans** analyze particular devices on a network,like searching for misconfigurations on a firewall.

6. **Comprehensive scans** analyze *all* devices connected on a network. This includes operating systems,user databases and more.

#### Patch update -
A patch update is a software and operating system update that addresses security vulnerabilities within a program or product. Patches usually contain bug fixes that addresses common security vulnerabilities and exposures.

# Two types of updates:
1. #### Manual updates -
A manual deployment strategy relies on IT departments or users obtaining updates from the developers. Home office or small business environments might require you to find, download, and install updates yourself. In enterprise settings, the process is usually handled with a configuration management tool. These tools offer a range of options to deploy updates, like to all clients on your network or a select group of users.  

**Advantage:** An advantage of manual update deployment strategies is control. That can be useful if software updates are not thoroughly tested by developers, leading to instability issues.

**Disadvantage:** A drawback to manual update deployments is that critical updates can be forgotten or disregarded entirely.

2. #### Automatic updates -
An automatic deployment strategy takes the opposite approach. With this option, finding, downloading, and installing updates can be done by the system or application.
Certain permissions need to be enabled by users or IT groups before updates can be installed, or pushed, when they're available. It is up to the developers to adequately test their patches before release.

**Advantage:** An advantage to automatic updates is that the deployment process is simplified. It also keeps systems and software current with the latest, critical patches.

**Disadvantage:** A drawback to automatic updates is that instability issues can occur if the patches were not thoroughly tested by the vendor. This can result in performance problems and a poor user experience.

# End-of-life software:
1. Sometimes updates are not available for a certain type of software known as end-of-life (EOL) software.
2. All the software has a lifecycle. It begins when it's produced and ends when a newer version is released. At that point, developers must allocate resources to the newer versions, which leads to EOL software.
3. While the older software is still useful, the manufacturer no longer supports it.
4. The risks that EOL software presents continues to grow as more connected devices enter the marketplace.
5. For example, there are billions of IOT devices,like smart light bulbs,connected to home and work networks.
In some business settings, all an attacker needs is a single unpatched device to gain access to the network and cause problems.

# Penetration Testing:
1. A penetration test,or pent test, is a simulated attack that helps identify vulnerabilities in systems, networks, websites,applications and processes.
2. The simulated attack in a pentest involves using the same tools and techniques as malicious actors in order to mimic a real life attack.
3. Since a pen test is an authorized attack, it is considered to be a form of ethical hacking.
4. Unlike a vulnerability assessment that finds weaknesses in a system's security, a pen test exploits those weaknesses to determine the potential consequences if the system breaks or gets broken into by a threat actor.
5. **For example**, the cybersecurity team at a financial company might simulate an attack on their banking app to determine if there are weaknesses that would allow an attacker to steal customer information or illegally transfer funds.

### Teams - 
1. **Red Team** tests simulate attacks to identify vulnerabilities in systems,networks or applications.
2. **Blue Team** tests focus on defense and incident response to validate an organization's existing security systems.
3. **Purple Team** tests are collaborative improving security posture by combining elements of red and blue team exercises.

### Pentetration Testing Strategies:
1. **Open-box testing** is when the tester has the same privileged access that an internal developer would have, information like system architecture,data flow and network diagrams. This strategy goes by several different names, including internal, full knowledge, white-box, and clear-box penetration testing.

2. **Closed-box testing** is when the tester has little to no acccess to internal systems, similar to a malicious  hacker. This strategy is sometimes referred to as external, black-box, or zero knowledge penetration testing.

3. **Partial knowledge testing** is when the tester has limited access and knowledge of an internal system—for example, a customer service representative. This strategy is also known as gray-box testing.

### Becoming a penetration tester -
Network and application security

Experience with operating systems, like Linux

Vulnerability analysis and threat modeling

Detection and response tools

Programming languages, like Python and BASH

Communication skills

### Bug Bounty programs:
Organizations commonly run bug bounty programs which offer freelance pen testers financial rewards for finding and reporting vulnerabilities in their products. Bug bounties are great opportunities for amateur security professionals to participate and grow their skills. 

HackerOne - bug bounty platform
