Repo for researching regarding Q stuff

Links here:


```
Task Force Patriots
Calling all Patriots -- Only for the brave
Operation: Save the children

Documents:
  Previous Work: https://8kun.top/qresearch/res/2371258.html#2371258
    -- imply pixelknot takes sha256 to unlock the photos?
    -- say to use older version of pixelknot that newer authors stripped an important part from it?
  Q Drops: https://qagg.news/
	   https://qposts.online/
  Code use mega passworld file:
     -- Passwords should be reflected, caps, etc
        -- Example: PRES45 would also be pres45, also 54serp, etc

Steps to decipher a password:
  ???  -- Need clear steps on this


Good candidate to decipher:
  Key (Most important): https://qagg.news/?q=%7BD11%2F7%2F2017%7D
  Key is probably used to decrypt all other pictures?
  Recent: https://t.me/georgenews/655


Leads:
  Wayfair Pedo Store: https://www.wayfair.com/brand/bnd/isabelline-b48131.html		(look at the logo)
    -- See https://greatawakening.win/p/12hRQIaFOd/these-extremely-expensive-blood-/c/
    -- stegdetect on these?
  Castle Rock:
    -- Anon mentioned Antartica has a Castle Rock point.
  Any possible encrypted photo:
    -- Could have the photo as a key of sorts
       -- How do we convert the photo to a key?
    -- Could have something hidden in the photo
       -- How do we get the data out of the photo?
    -- Could have something hidden in the code of the web page.
  *Working Theories*:
    -- QR Code - 20% reduction, 4 black corners:
       -- Take a Q picture, say the key:
       -- Use pixelknot to put a password into it that gives it a black corner.
       -- Maybe reduce the picture by 20% before or after the 4 black corners.
       -- Then use OPENPUFF to decrypt the message
       -- Code be QR code.
    -- Stenography - 20% reduction, 4 black corners:
       -- Mash multiple Q pictures?
       -- in order to get the stegno, we need to set up the correct parameters. Q mentioned these in drops.
       -- making python program for this:
          -- see https://www.tutorialspoint.com/working-with-images-in-python for basics
          -- pip install pillow (or use package manager)
    -- Stenography - by itself:  
    -- Pictures: are the evidence themselves , leaked?

    -- Overall Picture:
    -- Key: leads to the evidence itself.
       -- Jeffrey epstein photos
       -- everything declassified
       -- unsure
    -- Map
       -- our objective is learn to read the map
       --


Code bases:
  Pixelknot: https://github.com/guardianproject/PixelKnot
     -- oldest update from two years ago
  F5-Stegnography (is tha 8kun was using?): https://github.com/matthewgao/F5-steganography
     -- run via command line. see not on using decrypt ie d
     -- can we make this into a brute force script via perl?
  jphide and seek: https://github.com/h3xx/jphs
     -- might get this error when running: install correct correct jpeg package:
	https://serverfault.com/questions/739363/wrong-jpeg-library-version-library-is-62-caller-expects-80
  stagdetect: https://github.com/abeluck/stegdetect
     -- unmaintained
     -- to setup:
        -- git clone https://github.com/abeluck/stegdetect
        -- cd stegdetect
        -- ./configure
		-- errors occured for me here on Whonix with aclocal.m4 -- needed to `touch aclocal.m4` and `rm -rf build/*` and reconfigure
                -- see: https://stackoverflow.com/questions/33278928/how-to-overcome-aclocal-1-15-is-missing-on-your-system-warning
        -- make
   PixelUnKnot:
      -- listed by the 8kun previous research
           -- https://github.com/banona/PixelUnknot
   exiftool:
      -- exiftool on space force says tags are off.
   stego-toolkit:
	https://github.com/DominicBreuker/stego-toolkit
   https://www.nsa.gov/resources/everyone/ghidra/


Notes Per User:
    -- X... believes detection algorithm is incorrect
       the images have embedded thumbnails and a lot of exif data that is unusual
       From SqueezeOrSqooze: what are the next steps if you are correct?
       Stegdetect found something as well. Did stegdetect find stuff in the wayfair photos? Is that the rug photo?
       Says image embedded with jphide --> big?
       Added jphide link under code bases
       Steps to reproduce:
          -- clone stegdetect. clone jphide. download image

    -- Y - got pixelknot to 60% but crash. Does pixelknot even work? Used photo from drop 869.
       Used password: EA29DD13-F16F-4580-9DC8-0D69
       Password was image name -> except the three dots at the end of it were odd (so in telegram desktop app, I think the filename
       is fully flushed out. still odd though). Drops points to IDEN + 1 (letters, I=9, D=4, E=5, N=14 which sum to 68 + 1 is 69).
       Replaced the three dots with 69. Took it the highest we have seen to 60% and then crashed
       		-- Subnotes: pixelknot seems to crash a lot. Does this happen for the wrong password or is the app bunk. Can F5-Stego git
		   repo linked to replace pixelknot. Seems the 8kun thread thought that was viable.
	Yalso wants to stick with Q photos (no memes). Good. i would also suggest GEORGENEWS pictures as I believe GEORGENEWS is the current Q.
        (begs question why did Q drop his password).
        Y OPENPUFF to trim down pictures by 20% per Q posts #4660, read drops 4658-4663


Questions:
  -- Is Q trying to leak confidential info? Why something like Castle Rock a place in Antartica?
  -- Why all the satantic symbols?
  -- What is the key, keystone, and map for?
  -- Why would Q encode stuff for us to decrypt? Why is it encrypted in such a complex way?



Suggested tools / protocals:
   -- VPN at very least
   -- Tor suggested -- do not use with VPN
   -- QubesOS, Whonix, at least Linux on PC (Windows is shaky, run oWo Windows shut up to disable most telemetry)
   -- grapheneOS on mobile (requires specific google pixel phones) or at least a de-googled phone -- use orbot for tor on mobile
   -- secure methods of communication
   -- do not leak personal identity as best as possible
   -- workflows
      -- command line or programs
      -- could use android in a virtual emulator for pixelknot as suggested by one user
      -- will we need a code repo?
      -- Improvement to workflow:
  		-- nextcloud?
  		-- any git repos?


Previous Research:
  -- It does look like someone got decoding to work: See 2372349 on 8kun research page
  -- IMPORTANT: post 2373244 says:
     "... if we crack image it might give us a clue on the passwords for the others." My thoughts exactly. That is the key
     -- see https://qagg.news/?q=%7BD11%2F7%2F2017%7D
  -- See post 2376493 -- links to code to decrypt?
  -- See posts 2376582 and 2376618: PixelKnot uses the last 1/3 of the password for F5 encryption. What of the other 2/3rds?
     -- "Rest is the AES encryption layer"
  -- Wonder why 2376861 says 2376835 is glowing.
  -- Potentially huge -- did they decode something here ?: https://8kun.top/qresearch/res/2380204.html#2380591 post 2380591
  -- See 2382513: is the method of decryption to use the old pixelknot version (not on google play store) minus the two sketchs
     commits. Per post, we want to do statistical analysis of the JPEG coefficients. This was something someone else brought up
     as well.
  -- See 2387734: pixelknot is indeed a trash app. would only media use to. proof of collusion?


1 - Install Genymotion or Bluestacks or use VirtualBox. Create Android 4.4 device.
2 - Get / install PixelKnot app via fdoid. V1.01
  - Use it to create encrypted pic and send pics via email or bluetooth  -- must have imap or pop3 enabled for email account
  - Make note of password and secret text. For this example password is Abcd1234
3 - Install Java (we are using openJDK11 ). Decrypt using f5.jar from google and last 1/3 of password. See notes on how to compute.
    f5.jar : https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/f5-steganography/f5.jar
  - Command is below. -p is last 1/3rd of password.
    - specifically password for the f5 part is the length of the example password, say Abcd1234    (8) divided by 3 (2.XXX),
      rounded down (2), times 2 (4), then it is the length (8) minus that (4) -> use last 4 letters of password
  - Using openjdk 11.0
      'java -jar f5.jar x -p 1234 -e out.txt pktestpic.jpg'
  - Then view out.txt will give output of
     ----* PK v 1.0 REQUIRES PASSWORD ----*ciphertext
Best guess for next step - feed the ciphertext into the aes gcm algo

```

```
Voat
Many of you have heard of the now gone Voat.co. While the site went dark on 25 Dec 20, all of the research still lives on at SearchVoat.co.
Personally, I believe Voat was used as an ingestion point for all of the research into PG and Q, used to tune the artificial intelligence on a quantum computing system. Voat was the only research site "sanctioned" by Q - voat.co/v/QRV.
Regardless, SearchVoat.co is a powerful research tool, providing the researcher with many key words, starting points, and topical digs into content censored or memoryholed.

Here are a few topics:
Comet Ping Pong: https://searchvoat.co/search.php?t=comet+&s=pizzagate&p=100
Pegasus Museum: https://searchvoat.co/search.php?t=pegasus&s=pizzagate
Wikileaks Pizza Code: https://searchvoat.co/search.php?t=wikileaks&s=pizzagate&p=100
MK Ultra: https://searchvoat.co/search.php?t=mk&s=pizzagate&p=4
Adrenochrome: https://searchvoat.co/search.php?t=adrenochrome&s=pizzagate&p=1
Illuminati: https://searchvoat.co/search.php?t=illuminati&s=pizzagate&p=5
Pizza: https://searchvoat.co/search.php?t=pizza&s=pizzagate
Epstein: https://searchvoat.co/search.php?t=epstein&s=pizzagate&p=100
```

```
8Kun


```

```
GA.win

```


```
www.awoken.win


```
