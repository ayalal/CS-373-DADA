# Final Write-Up Hack The Box
--------------------------------------------------------------------

## Obtaining an Account (5 pts.)
After reaching the invite page I immediately examined the web page through the inspector tools providing by Google Chrome to see if any scripts were running in the background that could link to a invite code generator or hint at one. Within the inspector was a inviteapi.min.js script which caught my attention. I then opened up the file in the sources tab to insepct the code where there was a defined function called makeInviteCode that could be run within the Javascript console provided by Chrome. 

<img src="HackTheBoxInvite.png" alt="failed" class="inline"/>
<img src="inviteFunction.png" alt="failed" class="inline"/>

Knowing that the funciton could be ran I made call to it within Chrome using the built in console to see what output would be provided as a result. After running the result contain encrypted text which was encrypted using Base64 encoding scheme. Knowing the encryption scheme I copied the provided data and went looking for a text decoder that has Base64 as an option. 

<img src="inviteResult.png" alt="failed" class="inline"/>

When I found a decoder I entered in the cipher text provided from the function set to decode from Base64 and let the decoder do its work. After being decoded the message stated 'In order to generate the invite code, make a POST request to /api/invite/generate'.

<img src="inviteDecode.png" alt="failed" class="inline"/>

I then made a POST request following the format suggested by the cipher text and was provided the result below.

<img src="invitePost.png" alt="failed" class="inline"/>

With the newly provided cipher text from the API used by 'hack the box' I returned to the decoder and decoded the cipher text from the API which in return gave me the generated invite code for the website. 

<img src="inviteCode.png" alt="failed" class="inline"/>

After entering my code I was able to register an account with 'Hack the Box' and continued to the challenges!

## First Challenge Topic-Reverse Name-Snake
Since I had no idea where to start I chose the first file which dealt with reversing challenges. I then chose the easiest listed challenge available so that I could get a feel for what the challenges in 'Hack the Box' would be like. 
