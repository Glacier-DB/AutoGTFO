# AutoGTFO
A command line tool designed to find privilege escalation opportunities on Linux systems, using <a href="https://gtfobins.github.io/">GTFObins.</a> Written in Python3.

Firstly, a huge shout out to <a href="https://gtfobins.github.io/">GTFObins.</a> If you haven't checked it out already, it's an amazing resource for unix privesc and living off the land attacks.

This script essentially uses the "find" command to search for executable binaries on the system, and checks them against <a href="https://gtfobins.github.io/">GTFObins</a>. The script can also check the executing user's sudo capabilities.

I decided to develop this tool to streamline <a href="https://haxf4rall.com/2019/06/29/ctf-guide/">CTF</a> challenges.

# Prerequisites
* Python3 installation
* Python3 Requests Module
* Linux operating system
* An internet connection

# Installation
Get the script on your local machine by either:

1) Clone the respository:
(Recommended: change git core.autocrlf to input!)
<pre>git config --global core.autocrlf input</pre>
<pre>git clone https://github.com/nochhacks/AutoGTFO</pre>

2) Download the ZIP file directly from the "Code" drop down on the page, and unzip it.

3) Give the script execute permissions so you can run it from the console.
<pre>cd /path/to/AutoGTFO</pre>
<pre>chmod +x AutoGTFO</pre>

4) If you don't already have the python requests module, install it like so:
<pre>pip3 install requests</pre>

# Usage

<pre>
USAGE: ./AutoGTFO {OPTIONS}

optional arguments:
  -h, --help            show this help message and exit
  -s, --sudo            Includes a sudo privilege check (sudo -l), may require
                        passwd input
  -l, --list-functions  List all possible functions supported by binaries
</pre>

