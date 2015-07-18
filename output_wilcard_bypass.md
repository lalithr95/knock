# Scanning alice.it (with wildcard enabled) #

## Before ##
I try to scan domain **alice.it** but knock tells me that the wildcard is enabled.
```

*$ ./knock alice.it*

Knock v1.5 by Gianni 'guelfoweb' Amato ( http://knock.googlecode.com )

[+] Testing domain
www.alice.it           217.169.121.227
[+] Dns resolving
Domain name               Ip address              Name server
No address associated with hostname alice.it
[+] Testing wildcard

<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>404 Not Found

Unknown end tag for &lt;/title&gt;




Unknown end tag for &lt;/head&gt;

<body>
<h1>Not Found

Unknown end tag for &lt;/h1&gt;


<p>The requested URL / was not found on this server.

Unknown end tag for &lt;/p&gt;




Unknown end tag for &lt;/body&gt;



Unknown end tag for &lt;/html&gt;




Wildcard enabled! Try with -bw option
Example: knock -bw 404 alice.it
```
## After ##

The server responded with an HTML page that contains the error **404**. Ok, I can use the "-bw" followed by the string to exclude all pages that contain. Happy :-)
```

*$ ./knock -bw 404 alice.it*

Knock v1.5 by Gianni 'guelfoweb' Amato ( http://knock.googlecode.com )

[+] Testing domain
www.alice.it           217.169.121.227
[+] Dns resolving
Domain name               Ip address              Name server
No address associated with hostname alice.it
[+] Bypass wildcard
blog.alice.it
cc.alice.it
chat.alice.it
community.alice.it
device.alice.it
forum.alice.it
help.alice.it
images.alice.it
irc.alice.it
m.alice.it
mail.alice.it
mail2.alice.it
messenger.alice.it
mobile.alice.it
pg.alice.it
search.alice.it
shopping.alice.it
w.alice.it
ww.alice.it
www.alice.it
www-.alice.it

Found 21 subdomain(s) in 1326.1 second(s)
```