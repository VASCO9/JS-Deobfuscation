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


EXCERSICE:

vasco@PRUEBASVASCO:~$ curl -s http://134.209.191.224:30331 -X POST
</html>
<!DOCTYPE html>

<head>
    <title>Secret Serial Generator</title>
    <style>
        *,
        html {
            margin: 0;
            padding: 0;
            border: 0;
        }

        html {
            width: 100%;
            height: 100%;
        }

        body {
            width: 100%;
            height: 100%;
            position: relative;
            background-color: #6fb3eb;
        }

        .center {
            width: 100%;
            height: 50%;
            margin: 0;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            color: white;
            font-family: "Helvetica", Helvetica, sans-serif;
            text-align: center;
        }

        h1 {
            font-size: 144px;
        }

        p {
            font-size: 64px;
        }
    </style>
    <script src="api.min.js"></script>
</head>

<body>
    <div class="center">
        <h1>API Keys</h1>
        <p>API Keys control panel</p>
    </div>
</body>

</html>vasco@PRUEBASVASCO:~$ curl -s http://134.209.191.224:30331/keys.php -X POST
4150495f70336e5f37333537316e365f31355f66756evasco@PRUEBASVASCO:~$ echo 4150495f70336e5f37333537316e365f31355f66756e | base64
NDE1MDQ5NWY3MDMzNmU1ZjM3MzMzNTM3MzE2ZTM2NWYzMTM1NWY2Njc1NmUK
vasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$ curl -s http://134.209.191.224:30331/keys.php -X POST -d key="4150495f70336e5f37333537316e365f31355f66756e"
4150495f70336e5f37333537316e365f31355f66756evasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$ echo 4150495f70336e5f37333537316e365f31355f66756e | xxd -p -r
API_p3n_73571n6_15_funvasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$
vasco@PRUEBASVASCO:~$ curl -s http://134.209.191.224:30331/keys.php -X POST -d "key=API_p3n_73571n6_15_fun"
HTB{r34dy_70_h4ck_my_w4y_1n_2_HTB}vasco@PRUEBASVASCO:~$
