---
sidebar_position: 1
---

# Foreword
Once a ransomware operator has gotten onto your network, they want to achieve predictable objectives. In most cases, the attacker seeks:

-** Persistence **- After gaining an initial foothold, the attacker will attempt to sink an anchor into the victim network that will enable them to come back and maintain access. This is commonly done by configuring the first infected machine to call back to the attacker even if it’s rebooted.  

-** Escalate privileges** - Unless the attackers get lucky, the account that initially fell victim to the intrusion will have insufficient privileges on the network. Attackers will seek to elevate themselves to a higher privilege level, which will help them access more systems and spread wider into the target in the next step…  

-** Lateral Movement** - Once the attacker has stolen access to higher privileges, they will begin to move around the network, infecting more machines and hoovering up data.  
  
 -**Exfiltration **- By this point in the kill chain, the bad guys might siphon some data out of the network, which will help extort the victim further down the line.  

-**Deployment **- Finally, attackers will deploy ransomware with creative techniques that ensure maximum damage and disruption.

It is important to note that PreventRansomware does not expect, want or require you to become an expert in the following attack tactics. We instead wish to instil knowledge that you don't need to be a cyber security scientist to win at defending. Getting the basics right and understanding the mechanics of each category of tactic will go a _very, very_ long way. 

Fortunately for us defenders, most tactics leave indicators in their wake that we can monitor and alert on but ingesting, parsing and writing alert logic for log data at scale can be a taxing task because there are many relentlessly changing methods and security tooling can be complex, especially in a Windows environment. PreventRansomware continues to stress that it may not be suitable for all teams to build out bespoke detection capabilities, and that’s OK. If you have the budget to deploy some form of EDR tool with pre-baked prevention, it is most likely worthwhile, but please don’t despair if not; as previously mentioned, good security best practices go a long way and are often implementable without cost because most of the gains can be achieved by tweaking settings in existing technologies as we saw in the previous chapters.

  
