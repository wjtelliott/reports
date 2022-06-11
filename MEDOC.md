# Ukrainian tax-filing software malware

- What type of attack was this?

This type of attack would be considered a worm, or self-spreading malware attack. It is
believed to have initially spread through an email, but soon attached itself to a
self-updating software by an accounting firm, MEDoc, located in Ukraine. The source of the
attack is still unclear, but the company MEDoc currently denies responsibility of the
creation or intentional spreading of this worm. Around 80% of all infections were in Ukraine,
with another 9% in Germany. 

- How was the vulnerability discovered and the attackers exploit this?

This worm uses a variety of vulnerabilities. It seems as this worm attaches and infects
the companies automatic software updating tools used in their accountant programs. Once
the computer is infected, it will attempt to spread to other computers on the same network.
This is achieved using an exploit called EternalBlue through an SMB or Server Message Block.
Once the other computers are infected, it will attempt to hijack admisitrator tools with
elevated user access for remotely controlling the users PC and installing software.
Lastly, the infected computer's Master File Table is attacked to confuse the location indexes
of files on the PC. After a short time, the computer will reboot and give a final ultimatum
to the user: Provide a payment to unlock and access your information.

- Were there security measures that could have been taken in order to prevent this attack?

Unlike usual worms, that require the users to mistakenly click on a link in an email or
message, this attack is carried out through the software update tool from various companies.
Assuming that they aren't already, the update tool could use verification methods using SHA
or MD5 before downloading and installing new updates. If this was used and the attackers had
bypassed this as well, very strict testing on update verification and access to the update
pushes could have helped. All in all, attackers will crack these and find a way through. A
two-step verification requiring multiple users to review and make changes to production
updates before they are able to be uploaded may have been the best route.
