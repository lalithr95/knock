# Introduction #

Knock allows you to scan subdomains, Transfer Zone discovery, Wildcard testing with internal or external wordlist.

This program is self contained, doesn't need to be installed in any particular location. All it needs is a recent version of Python 2.x

Only for use the <a href='http://en.wikipedia.org/wiki/DNS_zone_transfer'>Zone Transfer</a> option (**-zt**) you must install the module <a href='http://www.dnspython.org/'>dnspython</a>, otherwise you can do without. If the name server allows zone transfers to occur, all the DNS names and IP addresses hosted by the name server will be returned in human-readable ASCII text.

# Usage #
> ```
$ python knock.py <option> <url>```

### Rapid Scan ###
> <b>Scanning with <u>internal</u> wordlist:</b>

> ```
$ python knock.py <url>```

> <b>Scanning with <u>external</u> wordlist:</b>

> ```
$ python knock.py <url> <wordlist>```


### Options ###

> <b>-zt</b> <u>Zone Transfer discovery:</u>

> ```
$ python knock.py -zt <url>```

> <b>-dns</b> <u>Dns resolver:</u>

> ```
$ python knock.py -dns <url>```

> <b>-wc</b> <u>Wildcard testing:</u>

> ```
$ python knock.py -wc <url>```

> <b>-bw</b> <u>Wildcard bypass:</u>

> ```
$ python knock.py -bw <stringexclude> <url>```

## Executable on Linux ##
> <a href='http://code.google.com/p/knock/downloads/list'>Download knock</a> **tar.gz** archive and extract file _knock.py_

> From shell command:
> ```
$ sudo cp knock.py /usr/local/bin/knock
$ sudo chmod a+x /usr/local/bin/knock ```

> Now you can use knock as shown in the examples.

## Executable on Windows ##
> <a href='http://code.google.com/p/knock/downloads/list'>Download knock</a> **zip** archive, extract folder and use file _knock.exe_

> Required: <a href='http://www.python.org/ftp/python/'>Python 2.x</a> and <a href='http://www.dnspython.org/kits/1.6.0/dnspython-1.6.0.win32.exe'>Dnspython</a>

# Examples #
> <b>Scanning with <u>internal</u> wordlist</b>

> ```
$ ./knock domain.com```

> <b>Scanning with <u>external</u> wordlist</b>

> ```
$ ./knock domain.com wordlist.txt```

> <b>Zone Transfer discovery (-zt)</b>

> ```
$ ./knock -zt domain.com```

> <b>Dns resolver (-dns)</b>

> ```
$ ./knock -dns domain.com```

> <b>Wildcard testing (-wc)</b>

> ```
$ ./knock -wc domain.com```

> <b>Wildcard bypass with <u>internal</u> wordlist (-wc)</b>

> ```
$ ./knock -bw stringexclude domain.com```

> <b>Wildcard bypass with <u>external</u> wordlist (-wc)</b>

> ```
$ ./knock -bw stringexclude domain.com wordlist.txt```

## Sample stdout to file ##
> This will cause the ouput of a knock to be written to a text file

> ```
$ ./knock domain.com > output.txt```


_You do not understand how to use knock? Back to play with the Xbox!_

# Author #

> Gianni '<a href='http://www.guelfoweb.com'>guelfoweb</a>' Amato

# Contact #

> guelfoweb@gmail.com

> <a href='http://twitter.com/guelfoweb'>Twitter @ guelfoweb</a>