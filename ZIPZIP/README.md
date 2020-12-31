**Challenge Description:**
  My friend sent me this zip file... 
  He is a prankster and compressed the file a LOT of times...
  I don't know how to make this go quickly and I don't have the time... 
  At least he told me the password is "pass".
  Can you please help? 

**Challenge Solution:**
  It was immediately clear that this file had been zipped up and password protected 50 times with the password of pass. 
  
 ```python3
  #!/usr/bin/env python3
  import zipfile
  import sys

  ext = ".zip"
  password = "pass"


  for i in range(50, -1, -1):
    if i < 10:
      i = "0" + str(i)
    filename = str(i) + ext
    sys.stdout.write("\r[*] - UNZIPPING " + filename)

    with zipfile.ZipFile(filename) as file:
      file.extractall(pwd = bytes(password, 'utf-8'))


  with open("flag.txt", "r") as f:
    print("\n" + f.read())
	
 ```
