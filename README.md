# ngxing (windows 10 tested) + mapped worldwide.bose.com configuration with ssl certificate valid till 19 May 2023

##### Note: This work was done based on the https://github.com/bosefirmware/ced/issues/4 thread so read it for more information in case you need help!

### Instructions
**1. extract the nginx.zip archive to c:/ (c:/nginx) to make it work without modification of the nginx.conf file.**

**2. go to c:/nginx and install rootCA.crt to Trusted Authorities**

**3. replace (or modify if needed) C:\Windows\System32\drivers\etc\hosts with the 'hosts' file in this repo**

**4. start c:/nginx/nginx.exe and you should be able to open https://worldwide.bose.com/connected_device in your browser and see lines like  URL=https://raw.githubusercontent.com/bosefirmware/eb/master/drowsy_charger/index.xml with no ssl errors. Just make sure you see raw.githubusercontent.com/bosefirmware there, this indicates the nginx proxy is doing its job!**

**5. open https://btu.bose.com/ and install the updater app (if you don't have it already) and you should be able to connect to your headphones/etc**

**6. if the above works press a d v up down and you should see a "super secret" menu allowing you to choose the exacted firmware version you need to install**

PS: I was able to revert my Bose QC35i to firmware 1.0.6 from 3.0.3 on Win10/Edge with this setup (:
