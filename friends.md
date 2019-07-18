# CTF Name – Challenge Name

* **Category:** category
* **Points:** points

## Challenge

> Having snooped around like the expert spy you were never trained to be, you found something that takes your interest: "Cookie/www.FriendSpaceBookPlusAllAccessRedPremium.com" But unbeknownst to you, it was only the 700nm Wavelength herring rather than a delicious cookie that you could have found. It looks exactly like a credential for another system. You find yourself in search of a friendly book to read.
> Having already spent some time trying to find a way to gain more intelligence... and learn about those fluffy creatures, you (several)-momentarily divert your attention here. It's a place of all the individuals in the world sharing large amounts of data with one another. Strangely enough, all of the inhabitants seem to speak using this weird pictorial language. And there is hot disagreement over what the meaning of an eggplant is.
> But not much Cauliflower here. They must be very private creatures. SarahH has left open some proprietary tools, surely running this will take you to them. Decipher this language and move forth!

## Solution
1. Run the vm progrma as follows ```python3 vm.py program```
2. Casually wait 5 hours for the url to load upto "http://emoji-t0anaxnr3nacpt4na.w" From there is can be assumed that the rest of the url is the same as the agriculture challenge so "http://emoji-t0anaxnr3nacpt4na.web.ctfcompetition.com/"
3. Investigating the code had us figure out the reverse engineering it would be a pain so we wait.
4. Following most of the cat links brought back nothing continue to wait on the website incase it gave the page with the url.
5. Giving on waiting the program after 3 whole days and google how to find hidden page urls. Then google the following ```site:http://emoji-t0anaxnr3nacpt4na.web.ctfcompetition.com``` Obviously is a writeup showed up in the search results dont click it
6. Looking through the links gave a link to ```http://emoji-t0anaxnr3nacpt4na.web.ctfcompetition.com/humans_and_cauliflowers_network/sarah.html``` browsing to her friend Ameber gave the flag
```
CTF{Peace_from_Cauli!}
```
