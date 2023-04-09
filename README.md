[DRAFT]

# Cybersec-102
A guide on how to safely use computers and the internet for businesses and paranoid people.

Chapters:
- HTML Cookies and CSRF
- fake-valid SSL certificates 
- VPN usage
- firewalls
- VMs
- Computer nuking
- BIOS conf
- encryption
- IDS
- DLP

## HTML Cookies and Cross-Site Request Forgery (CSRF) Attacks

![alt text](https://github.com/Cham0i/Cybersec-101/blob/main/Cybersec101/1.jpg)

An HTML Cookie is a piece of information of locally stored information that allows a website to individually identify your computer from other computers in your network. Without cookies, you would have to log in to every website and rebuild every shopping cart for each browsing session. Life without cookies would be tedious, but arguably safer. If someone stole your laptop and went to Amazon.com, the thief would have access to your Amazon account because the cookies on your computer would have them automatically logged in to your account. To keep yourself safe, only accept cookies on a trusted device, preferably one that can't be easily accessed by an authorized user (phones are easier to steal than desktops). Of course, some websites don't even give you the option to accept or reject cookies. In these circumstances, it's best to use an incognito tab so that the cookies used are destroyed once the incognito tab is closed. 

What if you live in a nice suburban neighborhood with a 0% change of being mugged? Should you still be vigilant about cookies? Absolutely; a hacker could use a Cross-Site Request Forgery (CSRF) attack to access your accounts by using your cookies. Back in yee old days, a hacker could sneak JavaScript code into an email that would run once the victim ran the HTML file (A.K.A viewed the email). Thus that hacker could send a request from your computer to your bank account requesting that it transferred 5K dollars to some offshore bank and the website would comply because the request came from your computer using your cookies. Fortunately, these types of attacks are not as common since most email clients have taken measures to stop JavaScript from sneaking into emails. Additionally many websites with sensitive information (such as banks) don't allow cookies to be stored anyways.

![alt text](https://github.com/Cham0i/Cybersec-101/blob/main/Cybersec101/2.jpg)
