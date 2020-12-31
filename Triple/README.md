**Challenge Description:**
    Author: @trevor#1933

    I was studying something called ASCII armor because I wanted to become better at encoding. 
    I was having fun until I realized I couldn't decode my message...

    Download the file below.
    
**Challenge Solution:**
    The attached file was downloaded and opened. It was found to contains the following:
    
    Ulc1amIyUnBibWNnWVNCdFpYTnpZV2RsSUdseklHRWdiRzkwSUc5bUlHWjFiaUIxYm5ScGJDQnBkQ0JwYzI0bmRDNGc= V20xNGFGb3pjM3BQVkd0M1RsZFJlVTFVVVRSYWFsSnRXa2RKTTFscVFYbE9WMDE1VFRKUk1rOUVVWGROUkU1cVdXNHdQUT09
    
    This looked like base64... The whole thing did not decode together - it is clear it is two base 64 strings (as can be discovered from the space inbetween, and the fiofirstrst string ending in '=') Plugging the first string into cyberchef gave: 'Encoding a message is a lot of fun until it isn't.'
    
    The second string was decoded in base64... to give another base64 encoded string... this was decoded, and another base64 string was given... which was decoded to FINALLY GIVE THE FLAG!
    
    flag{39905d2148f4fdb7b025c23d684003cb}
