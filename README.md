# snortalog

## Install on ubuntu 22.04

```
apt -y install libgd-dev

apt -y install cpanminus
apt -y install build-essential

```

```
cpanm GD
cpanm GD::Graph

```

```
cd deps
tar xzvf Net-Whois-IP-0.50.tar.gz
cd Net-Whois-IP-0.50_patched
perl Makefile.PL
make install
```

# Run

```
./snortalog.pl -1  -i -g png -o snort.html -report  -d  < alert_fast.txt
```

Copy `snort.html` to `/var/www/html/`

Open using browser

