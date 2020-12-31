**Challenge Description:**
    Author: @JohnHammond#6971

    We are chasing down a hacker, wannabeel33t and we watch to catch him red-handed.
    He keeps a low profile online, but he has to have some bad habits... 
    
    
**Challenge Solution:**
    As this was an OSINT challenge, the first thing to do was check for sites using the username 'wannabeel33t'
    
    Sites such as https://www.namecheckr.com/ and https://namechk.com/ are great for this, as well as the tool 'sherlock'.
    
    Although these sites give some false positives, the user's Reddit was found:
    https://www.reddit.com/user/wannabeel33t
    
    The user had no posts, although their bio had a strange string in...
    %66%6c%61%67%7b%36%36%62%31%35%33%34%37%63%35%38%63%39%31%64%31%39%33%37%66%30%62%34%30%65%39%37%33%64%33%66%36%7d
    
    URL decoding this with cyberchef gave the flag!
