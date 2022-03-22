# JS-Deobfuscation
cheat sheet

minifier: https://www.toptal.com/developers/javascript-minifier/
Obfuscation: 
https://beautifytools.com/javascript-obfuscator.php#
https://obfuscator.io/

Deobfuscator:
https://beautifier.io/
https://prettier.io/
http://www.jsnice.org/

javascript-minifier.

First, we will try BeautifyTools to obfuscate our code: https://beautifytools.com/javascript-obfuscator.php#

 We can copy this code into https://jsconsole.com, 
 
 Let's visit https://obfuscator.io. Before we click obfuscate, we will change String Array Encoding to Base64, as seen below:
 
 online beautifier our code : https://beautifier.io ; https://prettier.io/playground/
 
 to deofuscate we use: http://www.jsnice.org
 
 
 
 CURL
 
 Vasco@htb[/htb]$ curl -s http://SERVER_IP:PORT/ -X POST
 
 Vasco@htb[/htb]$ curl -s http://SERVER_IP:PORT/ -X POST -d "param1=sample"

 DECODING:
 
 base64
 echo https://www.hackthebox.eu/ | base64
 echo aHR0cHM6Ly93d3cuaGFja3RoZWJveC5ldS8K | base64 -d
 
HEX
echo https://www.hackthebox.eu/ | xxd -p
echo 68747470733a2f2f7777772e6861636b746865626f782e65752f0a | xxd -p -r

ROT13
echo https://www.hackthebox.eu/ | tr 'A-Za-z' 'N-ZA-Mn-za-m'
echo uggcf://jjj.unpxgurobk.rh/ | tr 'A-Za-z' 'N-ZA-Mn-za-m'
