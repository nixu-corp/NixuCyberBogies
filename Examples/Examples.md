## Examples

We have included two example systems that you can use for practicing threat modeling and playing games with the Cyber Bogie cards. Our examples also include, which Cyber Bogies could attack the system and how.

### Imaginary online shopping platform 'EasyShoppe'

EasyShoppe is a startup building an online shopping platform for sellers and buyers. In this concept, everybody can be a seller.

System description: [EasyShoppe-threat-modeling-example.pdf](https://github.com/nixu-corp/NixuCyberBogies/blob/master/Examples/EasyShoppe-threat-modeling-example.pdf)

Cyber Bogie | Potential attack or misuse case
----------- | -------------------------------
Script Kiddie "Jonne" | Jonne tries a list of known breached usernames and passwords to login to EasyShoppe. Jonne buys a cheap botnet-for-hire and runs a DDoS attack on EasyShoppe website to show off his skills.
Clueless Employee "Josh" | Josh is one of the few employees EasyShoppe has and does some administration work such as resetting passwords on top of marketing and accounting. While multitasking, Josh might accidentally reset somebody else's password or delete data, who knows...
Annoyed User "Hyacinth" | Hyacinth spotted something that sounded a bit odd in EasyShoppe's privacy statement, so she asked everyone she knew to send a data request to EasyShoppe, asking to get all information stored about them. This has now caused a lot of manual work for EasyShoppe because they haven't automated that collection process yet.
Social Engineering Victim "Patsy" | Somebody has created a fake account with Patsy's name, address, and other details on EasyShoppe. That somebody also ordered a bunch of goods from EasyShoppe using Patsy's identity to be paid later with an invoice. The identify thief snatched the delivery from Patsy's mailbox but left out the invoice for Patsy to pay...
Phishing Campaign Runner "Antonia" | Antonia exploits a known vulnerability on EasyShoppe site to get admin access on the site. She hides a phishing site on the webserver.
Malware Campaign Runner "Sergei" | Sergei exploits known vulnerability on one of the JavaScript libraries used by EasyShoppe and injects a malicious script that forces users to download ransomware when they visit the site.
Supply Chain Attacker "Lisbeth" | Lisbeth has added a typo-squatting package for one of the popular libraries, also used by EasyShoppe. Lisbeth's malicious library version steals information from the environment, including passwords.
Incompetent Developer "Derk" | Derk is one of the developers of the EasyShoppe site. Derk doesn't know anything about secure coding, so he uses insecure SQL query structures and forgets to add input validation. Derk's code contains lots of bugs and vulnerabilities.
State-sponsored Agent "Magic Hound" | Magic Hound has found out that some government agents they are after are frequent users of EasyShoppe, selling their hand-made woolen socks there. Magic Hound plans to compromise the site and set up a watering hole.


There are probably many other threat actors, as well! Who else you do you think could harm EasyShoppe's security on purpose or by accident?





### Imaginary surveillance camera system for home and small office use

With Acme.io's web camera, you can monitor your home or office even when you are away. The videos are stored in a cloud service and thus always available.

System description: [IoTCameraSystem-threat-modeling-example.pdf](https://github.com/nixu-corp/NixuCyberBogies/blob/master/Examples/IoTCameraSystem-threat-modeling-example.pdf)


Cyber Bogie | Potential attack or misuse case
----------- | -------------------------------
Script Kiddie "Jonne" | Jonne searches for vulnerable IoT cameras in Shodan. After finding a few, he downloads exploit code from ExploitDB to gain access to the cameras and record videos from other people's homes. Jonne tries a list of known breached usernames and passwords to gain access to the web application in the cloud.
Petty Thief "Kyle" | While no one is watching, Kyle snatches a couple of laptops and IoT cameras off the wall in a co-working office. If the price is right, somebody will buy this stuff second hand, no questions asked.
Opportunistic Passer-by "Kevin" | A local coffee shop has bought a web camera from Acme.io. Unfortunately, the camera was mounted within reach, so while the barista was busy steaming up lattes and cappuccinos, Kevin plugged in his laptop to the unused Ethernet port and found out that no one has changed the default credentials of the user interface. How annoying! Kevin decided to mess up with the configuration to teach a lesson.
Cloud Admin "Charlotte" | Charlotte watches the video recordings from various customers when she has some idle time. If somebody passes by and asks, she claims to "debug the video quality because of complaints." Charlotte shows the funniest videos to others in her team.
Clueless Employee "Josh" | Josh is a new hire in the operations team. Josh wants to convince everybody of his skills and is afraid to ask questions to not appear stupid. Josh is eager to do all tasks and appear efficient. Unfortunately, when tasked with key management, Josh efficiently distributed also all the private keys to everyone in the company. Database maintenance quickly turned into a disaster recovery exercise when Josh accidentally deleted half of the customer data. To err is human, right?
Supply Chain Attacker "Lisbeth" | Lisbeth's employer has recognized the Acme.io's growing business and tasked Lisbeth in infiltrating malicious code into the firmware of the cameras. Lisbeth has reverse-engineered the firmware and recognized open source libraries used by the product. The next step is to start contributing code to one of the libraries, and after gaining enough reputation, start making bigger changes and finally introduce an obfuscated backdoor. Lisbeth's employer can then use the backdoor to spy on all users, steal information, and plan crimes.
Incompetent Developer "Derk" | Derk is one of the developers of the system. Derk doesn't know anything about secure coding, so he forgets to add input validation or use any security features offered by the platform. Derk's code - both in the firmware and the cloud service web interface - contains lots of bugs and vulnerabilities.
Annoyed User "Hyacinth" | Hyacinth is not happy with the user experience on setting up her camera and is aggressively trying to reach help on Acme.io's feedback form, chat and support phone line. Because Hyacinth had to wait in queue for over five minutes, she wrote some angry tweets criticizing everything about Acme.io's products.
Social Engineering Victim "Patsy" | Patsy enters her Acme.io cloud credentials accidentally to a phishing site after getting a funny email about subscription renewal.
Evil Data Scientist "Aidan" | Aidan constantly looks for data dumps from data breaches in Pastebin and downloads them. Aidan compares this data to all the information Acme.io has collected about its customers and tries to re-identify people from anonymized data. Mostly for fun, but Aidan also shares juicy details to Madison from the marketing department. As a favor to Madison, recently, Aidan has also analyzed video contents of their customers to learn everything about who they are and how they live.
Profits First Marketeer “Mo” | Mo collects all metadata available and has persuaded Aidan, the Evil Data Scientist, to use machine learning to analyze all the customer videos in order to learn more about the environments the cameras are used in, the age and gender of people appearing in the camera feed and how big apartments the owners appear to have. Mo combines this data with everything from the marketing database and web site analytics to create targeted add campaigns in social media.
Stubborn Stalker “Sasha” | Sasha has installed Acme.io's security camera to his home. Sasha uses the camera to check up on what the kids and his wife are doing while he's away. "Why is that neighbor invited over coffee again!?" Sasha is not pleased.
Thoughtless Project Manager “Aisha" | Aisha is the project manager for next-generation camera products. New features are being developed based on Mo's analysis, and the aim is to reach totally new user groups. The team is already falling behind the schedules a bit, so Aisha pushes for working overtime and minimizing time spent on quality assurance. Ashley has also decided that security testing will not be needed this time "because there were no critical findings in the previous audit." Aisha also feels that privacy specialists are disrupting their feature development, so they are not invited, either.
Competitor R&D Engineer “Jin” | Jin is working for a competing IoT product company. Jin reverse engineers the camera firmware and finds out interesting things to copy, such as a neat way of compressing videos ("much more efficient than ours," Jin exclaims).




