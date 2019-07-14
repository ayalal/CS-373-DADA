## Week 3 Write-Up
Week 3 provided an introduction of malware defense presented by Craig Schmugar a security speicalist at McAfee. Material for the week consisted of malware first contact, detection, defensive tactics dependent on attack vector, signature analysis, and attack flows. Included in the material was a lab which utilized Yara which itself provides a rule-based approach to create descriptions of malware families based on textual or binary patterns. We also were introduced to the Cuckoo malware analysis tool which is used to create a sandbox for executing malicious files to study and understand malware. Following I will discuss in detail the material that was covered in week 3. 

### Malware Procedure 
Starting off the presentation was the overview of the steps malware takes to infect a desired host and/or system. Understanding the procedure is a building block in defense as providing the best defensive practices requires having knowledge on both sides of the playing field. General malware behavior steps are depicted in the diagram seen below (image provided by Craig Schmugar):

 <img src="MalwareProcedure.png" alt="" class="inline"/>

#### Malware Procedure Steps
1. First Contact - The medium or style of interaction utilized by the attacker to gain attention of a user so that the user will interact with the malicious software that is being presented which in cases can be through email, instant messaging, malvertising, poisoned search results, and physical access to a system. 

2. Local Execution - After establishing contact with the user local execution is acquired by the running unknowingly run an executable through a button or applicaiton. Local execution can also happen through browser exploitation via browser-based exploit kits or abusing features that are known on various software applications or even operating systems. 
