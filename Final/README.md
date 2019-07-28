# Final Write-Up Hack The Box
--------------------------------------------------------------------

## Obtaining an Account (5 pts.)
After reaching the invite page I immediately examined the web page through the inspector tools providing by Google Chrome to see if any scripts were running in the background that could link to a invite code generator or hint at one. Within the inspector was a inviteapi.min.js script which caught my attention. I then opened up the file in the sources tab to insepct the code where there was a defined function called makeInviteCode that could be run within the Javascript console provided by Chrome. 

<img src="HackTheBoxInvite.png" alt="failed" class="inline"/>
