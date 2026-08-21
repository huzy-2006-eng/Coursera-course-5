Attack surface - All the potential vulnerabilities that a threat actor could exploit.

Security hardening - The process of strenghtening a system to reduce its vulnerabilities and attack surface.

# Being prepared for anything:
Having a plan should things go wrong is important. But how do you figure out what to plan for? In this field, teams often conduct simulations of things that can go wrong as part of their vulnerability management strategy. One way this is done is by applying an attacker mindset to the weaknesses they discover.

Applying an attacker mindset is a lot like conducting an experiment. It's about causing problems in a controlled environment and evaluating the outcome to gain insights. Adopting an attacker mindset is a beneficial skill in security because it offers a different perspective about the challenges you're trying to solve. The insights you gain can be valuable when it's time to establish a security plan or modify an existing one.

# Simulating threats:
One method of applying an attacker mindset is using attack simulations. These activities are normally performed in one of two ways: proactively and reactively. Both approaches share a common goal, which is to make systems safer.

1. **Proactive simulations** assume the role of an attacker by exploiting vulnerabilities and breaking through defenses. This is sometimes called a red team exercise.

2. **Reactive simulations** assume the role of a defender responding to an attack. This is sometimes called a blue team exercise.

3. Proactive teams tend to spend more time planning their attacks than performing them. If you find yourself engaged in one of these exercises, your team will likely deploy a range of tactics. For example, they might persuade staff into disclosing their login credentials using fictitious emails to evaluate security awareness at the company.

4. On the other hand, reactive teams dedicate their efforts to gathering information about the assets they're protecting. This is commonly done with the assistance of vulnerability scanning tools. 

# Scanning for trouble:
 Security teams employ a variety of scanning techniques to uncover weaknesses in their defenses. Reactive simulations often rely on the results of a scan to weigh the risks and determine ways to remediate a problem.

 For example, a team conducting a reactive simulation might perform an external vulnerability scan of their network. The entire exercise might follow the steps you learned in a video about vulnerability assessments:

 1. **Identifcation:** A vulnerable server is flagged because it's running an outdated operating system(OS).
 
 2. **Vulnerability analysis:** Research is done on the outdated OS and its vulnerabilities.

 3. **Risk assessment:** After the due diligence, the severity of each vulnerability is scored annd the impact of not fixing it is evaluated.
 
 4. **Remediation:** Finally,the information that you've gathered can be used to address this issue.

During an activity like this, you’ll often produce a report of your findings. These can be brought to the attention of service providers or your supervisors. **Clearly communicating the results of these exercises to others is an important skill to develop as a security professional.**

# Threat actors:
1. **Competitors** refers to rival companies who pose a threat because they might benefit from leaked information.

2. **State actors** are government intelligence agencies.

3. **Criminal syndicates** refer to organized groups of people who make money from criminal activity.

4. **Insider threats** can be any individual who has or had authorized access to an organization’s resources. This includes employees who accidentally compromise assets or individuals who purposefully put them at risk for their own benefit.

5. **Shadow IT** refers to individuals who use technologies that lack IT governance. A common example is when an employee uses their personal email to send work-related communications.

# Hackers:
1. #### Unauthorized hackers:
An unauthorized hacker, or unethical hacker, is an individual who uses their programming skills to commit crimes. Unauthorized hackers are also known as malicious hackers. Skill level ranges widely among this category of hacker. For example, there are hackers with limited skills who can’t write their own malicious software, sometimes called script kiddies. Unauthorized hackers like this carry out attacks using pre-written code that they obtain from other, more skilled hackers.

2. #### Ethical hackers:
Authorized, or ethical, hackers refer to individuals who use their programming skills to improve an organization's overall security. These include internal members of a security team who are concerned with testing and evaluating systems to secure the attack surface. They also include external security vendors and freelance hackers that some companies incentivize to find and report vulnerabilities, a practice called bug bounty programs.

3. #### Semi-authorized hackers:
Semi-authorized hackers typically refer to individuals who might violate ethical standards, but are not considered malicious. For example, a hacktivist is a person who might use their skills to achieve a political goal. One might exploit security vulnerabilities of a public utility company to spread awareness of their existence. The intentions of these types of threat actors is often to expose security risks that should be addressed before a malicious hacker finds them.

# Advanced persistant threats:
An advanced persistent threat (APT) refers to instances when a threat actor maintains unauthorized access to a system for an extended period of time. The term is mostly associated with nation states and state-sponsored actors. Typically, an APT is concerned with surveilling a target to gather information. They then use the intel to manipulate government, defense, financial, and telecom services.

Just because the term is associated with state actors does not mean that private businesses are safe from APTs. These kinds of threat actors are stealthy because hacking into another government agency or utility is costly and time consuming. APTs will often target private organizations first as a step towards gaining access to larger entities.

# Access points:
1. Direct access, referring to instances when they have physical access to a system.

2. Removable media, which includes portable hardware, like USB flash drives.

3. Social media platforms that are used for communication and content sharing.

4. Email, including both personal and business accounts.

5. Wireless networks on premises.

6. Cloud services usually provided by third-party organizations.

7. Supply chains like third-party vendors that can present a backdoor into systems.

#### Attack vectors -
The pathways attackers use to penetrate security defenses.

**Practicing an attacker mindset -**
1. Identify a target.
2. Determie how the target can be accesssed.
3. Evaluate attack vectors that can be exploited.
4. FInd the tools and methods of attack.

**Defending the attack vectors**-
1. Educating the users.
2. Applying the principle of least privilege.
3. Using the right security controls and tools.
4. Building a diverse security team.

# Brute force attacks:
1. **Simple brute force attacks-** are an approach in which attackers guess a user's login credentials. They might do this by entering and combination of username and password that they can think of until they find the one that works.

2. **Dictionary attacks** are a similar technique except in these instances attackers use a list of commonly used credentials to access a system. This list is similar to matching a definition to a word in a dictionary.

3. **Reverse brute force attacks** are similar to dictionary attacks, except they start with a single credential and try it in various systems until a match is found.

4. **Credential stuffing** is a tactic in which attackers use stolen login credentials from previous data breaches to access user accounts at another organization. A specialized type of credential stuffing is called pass the hash. These attacks reuse stolen, unsalted hashed credentials to trick an authentication system into creating a new authenticated user session on the network.

**Tools of the trade:** 
Instead of dedicating the time to do this, attackers often use software to do the guess work for them. These are some common brute forcing tools:
1. Aircrack-ng
2. Hashcat 
3. John the Ripper
4. Ophcrack
5. THC Hydra


# Prevention measures:
1. #### Hashing and Salting:
Hashing converts information into a unique value that can then be used to determine its integrity. Salting is an additional safeguard that’s used to strengthen hash functions. It works by adding random characters to data, like passwords. This increases the length and complexity of hash values, making them harder to brute force and less susceptible to dictionary attacks.

2. #### Multi-Factor Authentication(MFA):
Multi-factor authentication (MFA) is a security measure that requires a user to verify their identity in two or more ways to access a system or network. MFA is a layered approach to protecting information. MFA limits the chances of brute force attacks because unauthorized users are unlikely to meet each authentication requirement even if one credential becomes compromised.

3. #### CAPTCHA:
A. CAPTCHA stands for Completely Automated Public Turing test to tell Computers and Humans Apart. It is known as a challenge-response authentication system. CAPTCHA asks users to complete a simple test that proves they are human and not software that’s trying to brute force a password.
B. There are two types of CAPTCHA tests. One scrambles and distorts a randomly generated sequence of letters and/or numbers and asks users to enter them into a text box. The other test asks users to match images to a randomly generated word. You’ve likely had to pass a CAPTCHA test when accessing a web service that contains sensitive information, like an online bank account.

4. #### Password policy:
1. Organizations use these managerial controls to standardize good password practices across their business. For example, one of these policies might require users to create passwords that are at least 8 characters long and feature a letter, number, and symbol. 
2. Other common requirements can include password lockout policies. For example, a password lockout can limit the number of login attempts before access to an account is suspended and require users to create new, unique passwords after a certain amount of time.
