# Kattymad
# v1.1
KattyMad is a tool designed to install and perform DDoS attacks over the onion protocol.  <br>
I started from a fork of "KARMA" but it was literally unmaintaned and was using old cookies concept and also network stack was performing worstly than expected.
So i started again and this time i found very useful the MHDDoS project. <br>
Im constantly editing this project because the aim is to create mass environments that can easily takeover onion networks.
Please, read the [TODO](TODO.txt) and help me.

(NB. Credits binary code is just a reverse from ascii common text)<br>
![kattymad](https://github.com/electr0lulz/kattymad/blob/e5438634e844787037fc47dc16806fb2bb05bc06/ddos/files/katty_1.png)


## Usage on Linux ##
Requirements:
You must use Python 3.9 or higher

Step:
```
git clone https://github.com/electr0lulz/kattymad.git
```
#Install Python3 modules
```
cd ~/kattymad/ddos/
pip3 install -r requirements.txt
sudo apt-get install -y golang-go
mkdir bombardier_tmp
cd bombardier_tmp
go mod init bombardier_tmp
go mod edit -replace github.com/codesenberg/bombardier=github.com/PXEiYyMH8F/bombardier@78-add-proxy-support
go get github.com/codesenberg/bombardier
cd ..
rm -r bombardier_tmp
```
or
```
pip install -r requirements.txt
```
#Install Chrome (or update it lastest version)
```
cd resources; wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo apt-get install ./resources/google-chrome-stable_current_amd64.deb
```
## EASYBUSY CAT? ##
```
cd ~/kattymad/ddos/; python3 setup.py
## Install Anonsurf through setup.sh or by yourself and get ready ##
```
## Example
```
Use DDoS Panel   : python3 kitty.py
Use command line : python3 kitty.py <method> <target> <thread> <time>
      └──────────> python3 kitty.py get https://example.onion 100 30
```
##
See you around.
[Electr0lulz](https://github.com/electr0lulz/)
##
