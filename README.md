# snortalog

Perl script that summarizes Snort logs

Original version: http://jeremy.chartier.free.fr/snortalog/

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
./snortalog.pl -1  -i -g png -o /var/www/html/snort.html -report  -d  < alert_fast.txt
```

Open using browser

