# AutoGTFO
A command line tool designed to find privilege escalation opportunities on UNIX systems, using <a href="https://gtfobins.github.io/">GTFObins.</a> Written in Python3.

This script essentially uses the "find" command to search for executable binaries on the system, and checks them against <a href="https://gtfobins.github.io/">GTFObins</a>. The script can also check the executing user's sudo capabilities.

# Prerequisites
* Python3 installation
* Linux operating system

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

# Usage

<pre>
USAGE: ./AutoGTFO {OPTIONS}

optional arguments:
  -h, --help  show this help message and exit
  -s, --sudo  Includes a sudo privilege check (sudo -l), may require passwd input
</pre>

