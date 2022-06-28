---
sidebar_position: 4
---

It's common for ransomware gangs to break into organisations simply by logging into a network with stolen, guessed or purchased credentials. Yes, that's right, **hackers are just logging in to your network to deploy ransomware.** 


### Updating your approach to passwords.

Traditional password policies such as _Eight characters, one special character, one uppercase character and forced expiry_ are no longer in favor because, in reality, they force users to set weak and easy to guess passwords. Old password policies like this are now considered _password anti-patterns._ 

- **Regular password expiry** - Regularly making a user change their password does more bad than good because it forces them into predictable patterns as they have to make their password memorable and accepted by the often narrowly defined password policy. A user’s password might currently be: “Summer69!” then, when the 90-day expiry comes around, it could be changed to “Summer420!”   

Microsoft has this to say:  
  
_Password expiration policies do more harm than good because these policies drive users to very predictable passwords composed of sequential words and numbers which are closely related to each other (that is, the next password can be predicted based on the previous password). Password change offers no containment benefits. Cybercriminals almost always use credentials as soon as they compromise them._  

- **Character Composition Requirements** - Forcing user passwords to contain a certain number of characters has a similar effect to forcing password expiry; weaker passwords are selected because the user is being forced to create a memorable but complex and therefore predictable password. (“Summer420!”)


They say there is an xkdc for everything, password policies are no exception:  

![PasswordImage][image-1]


Traditional password policies encourage  pass**words **that are easy for attackers to guess, brute force or crack. You should aim to create a modern password policy with length and longevity in mind, which means long and rarely expiring pass**phrases.** This concept sounds alien but is in line with guidance from leading cyber security experts at [government bodies][1] and [Microsoft:][2]

- **Maintain an 8-character or more minimum length requirement.** - **PreventRansomware recommends 16-characters**, which isn’t as bad as it sounds; using song lyrics or quotes from books forms long easy to, remember passphrases.

- **Don't enforce character composition requirements.** - For example, \*&(^%$ or a particular number of uppercase or lowercase letters.

- **Don't require mandatory periodic password changes for user accounts and mobile devices (like smart phone unlock pins)**

- **Ban common passwords** - Ban the use of common words like the names of seasons, celebrities and top common passwords like passwordpasswordpassword.[The NCSC provides a great list here.][3]

- **Enforce 2FA for all users.** - All user accounts must require two-factor authentication so that even if a password is compromised, the account won’t be. PreventRansomware strongly advises using physical security keys for accounts wherever possible or at least for high value administrator accounts. 

Thanks to its lack of expiry and long but non-complex requirements, this policy encourages strong pass**phrases** (instead of passwords) like song lyrics or passages from books, such as:

- Welcome to the jungle
- Hello my old friend
- Cheetos are the only way!

By changing to the above passphrase methodology, you will protect your organisation in multiple ways:

- Make it more challenging for attackers to get lucky when brute forcing logins to o365, Citrix, RDP and VPNs

- If an attacker does get into the network, longer passwords make lateral movement harder because offline password cracking becomes exponentially more time-consuming. The more time an attacker lingers on a network, the better.

**Added Bonus:** Improves your user experience by allowing them to use easy to type and remember passwords that they don’t have to rotate regularly. When a new user joins the company, you can tell them to use song lyrics or a passage from a book. They will be pleasantly surprised when you explain that they don’t need special characters. Also, the number of password reset tickets coming to the helpdesk will undoubtedly be reduced.








[1]:	https://www.ncsc.gov.uk/blog-post/the-logic-behind-three-random-words
[2]:	https://docs.microsoft.com/en-us/microsoft-365/admin/misc/password-policy-recommendations?view=o365-worldwide#password-guidelines-for-administrators
[3]:	https://www.ncsc.gov.uk/blog-post/passwords-passwords-everywhere

[image-1]:	https://imgs.xkcd.com/comics/password_strength.png