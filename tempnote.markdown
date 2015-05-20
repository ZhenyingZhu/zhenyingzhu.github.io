`du` diskusage.  

[ssh disable timeout](https://docs.oseems.com/general/application/ssh/disable-timeout)  

[Xfinity](http://customer.xfinity.com/help-and-support/internet/wireless-gateway-username-and-password?ts=2&CCT=53BA3D76CB1473BFF49C79FE4AA86DFF1EE2DE626F409A5997049C511025D7B2204A7E8531C277E2BCBE6703AA1E9BA0ED1CCE9EEACAF2E341918A8498DFEA031067DB3AB0550914C343562D66B6C738E6B3B5DD54EE00895D57EEDDAF943A63D722FEA4741C2635BFA54500D1EBC9A31BB35ED9541A9164590253CE54D95ED9   )

http://android.stackexchange.com/questions/2984/how-can-i-see-what-ip-address-my-android-phone-has  

http://stackoverflow.com/questions/4370960/what-is-attr-accessor-in-ruby  

http://stackoverflow.com/questions/151505/difference-between-a-class-and-a-module  

Port 0 is reserved.  

http://stackoverflow.com/questions/18193424/using-gsub-in-ruby-strings-correctly  
`dirname = File.basename(Dir.getwd)` find the current dir name in ruby  

[net bean extension](http://stackoverflow.com/questions/4134137/syntax-highlighting-php-shell-scripts-without-extension-in-netbeans)  
~/.netbeans/8.0.2/config/Services/MIMEResolver  


```
from subprocess import call
call("ls") # success
call("ls -l") # failed
call("ls .") # failed
call(["ls", "-l"]) # success
```

[Ruby XML](http://www.tutorialspoint.com/ruby/ruby_xml_xslt.htm)  
http://stackoverflow.com/questions/11315295/ruby-finding-elements-with-rexml  
http://www.germane-software.com/software/rexml/docs/tutorial.html  

[netstat](http://www.cyberciti.biz/faq/how-do-i-find-out-what-ports-are-listeningopen-on-my-linuxfreebsd-server/)  
[background](http://www.kossboss.com/linux---move-running-to-process-nohup)  
killall nc
Ctrl+z and fg
service lightdm stop to stop X windows.
who -b

sh-bang: 可用指令<code>env</code>，如#! /usr/bin/env python。

http://serverfault.com/questions/416222/concatenate-first-line-to-the-end-of-second-line-in-a-text-file

<code>grep -f Key.txt All.txt</code>
<code>sleep 60</code> to sleep 60 seconds.
<code>mail -s "test script" account@mail.com < /dev/null</code> send an email with title "test script".
<code>head -q -n 2 *.txt</code> Output several files without show the file name.* 
<code>sed -e 'N;s/\(.*\)n\(.*\)/\1\2/' </code> let the second lines append to the first lines. 

```
while read line; do
    SOMETHING
done < readfile
```

SSH:
```
eval `ssh-agent -s`
ssh-add ~/.ssh/id_rsa
ssh -A $HOST
```

Vim:
<code> set paste</code> and <code> set nopaste</code>

https://docs.python.org/2/library/subprocess.html  
http://effbot.org/zone/python-with-statement.htm  

[hping3](http://0daysecurity.com/articles/hping3_examples.html)  

`sudo yum -y --enablerepo="epel" install hping3`  

`$ dpkg -l | grep python`  

[DF flag](http://yurisk.info/2009/09/01/ping-setting-dont-fragment-bit-in-linuxfreebsdsolarisciscojuniper/)  
[wireshark](http://anonscm.debian.org/viewvc/collab-maint/ext-maint/wireshark/trunk/debian/README.Debian?view=markup)  

[Understand TCP](http://packetlife.net/blog/2010/jun/7/understanding-tcp-sequence-acknowledgment-numbers/)  

[nuttcp](http://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&ved=0CB8QFjAA&url=http%3A%2F%2Fwww.nuttcp.net%2F&ei=sHhKVbmcAcX8oATbkoCACw&usg=AFQjCNE2ezCkj69-haln6xb3TvnffAbx0w&bvm=bv.92291466,d.cGU)  and http://manpages.ubuntu.com/manpages/precise/man8/nuttcp.8.html  

http://lukaszwrobel.pl/blog/tmux-tutorial-split-terminal-windows-easily  

[split terminal](http://ubuntuforums.org/showthread.php?t=1813803)  

http://stackoverflow.com/questions/7188191/copy-file-over-tcp-socket-in-ruby-slow  

http://stackoverflow.com/questions/1661367/specify-packet-size-with-ruby-tcpsocket  

http://www.linuxquestions.org/questions/linux-networking-3/gigabit-ethernet-performance-643750/  

[web browser](http://www.tutorialspoint.com/ruby/ruby_socket_programming.htm)  

```
dd if=/dev/zero of=binary.dat bs=1c count=1 
dd if=/dev/zero oflag=append conv=notrunc of=binary.dat bs=1c count=1 #To append it to file
```

https://iperf.fr/#tuningtcp  

[TCP MTU](http://blogs.technet.com/b/onthewire/archive/2014/06/18/checking-your-tcp-packets-are-pulling-their-weight-tcp-max-segment-size-or-mss.aspx)  

[tcpdump](http://www.thegeekstuff.com/2010/08/tcpdump-command-examples/)

[eclipse](http://stackoverflow.com/questions/11596194/how-does-one-show-trailing-whitespace-in-eclipse)  

transport file (http://www.netperf.org/netperf/training/Netperf.html#0.2.2Z141Z1.SUJSTF.6R2DBD.2) 
```
netserver
netperf 127.0.0.1 -t udp_rr -- -r 1473,1473 -u

netperf -H remotehost -t UDP_STREAM -- -m 1024 # test udp
netperf -H remotehost -t TCP_RR

```

[python **args](http://www.saltycrane.com/blog/2008/01/how-to-use-args-and-kwargs-in-python/)  

[tcpdump](https://danielmiessler.com/study/tcpdump/)  

`iperf -s` on server and `iperf -c host` on client  

soft reboot: `sudo reboot`  

if `sudo -u user` failed, try `sudo logbash` and in the new bash, run that again.  

[find which shell](http://www.cyberciti.biz/tips/how-do-i-find-out-what-shell-im-using.html)  

[sudo -u](http://apple.stackexchange.com/questions/82438/allow-sudo-to-another-user-without-password)  

[shell wait background](http://unix.stackexchange.com/questions/124106/shell-script-wait-for-background-command)  

[MTU size](http://www.cyberciti.biz/faq/centos-rhel-redhat-fedora-debian-linux-mtu-size/)

[rename remote branch](http://www.benjaminlhaas.com/blog/locally-and-remotely-renaming-branch-git)  

[pull from fork](http://stackoverflow.com/questions/14383212/git-pulling-a-branch-from-another-repository)

[rebase](http://git-scm.com/book/en/v2/Git-Branching-Rebasing)

[change master branch](http://stackoverflow.com/questions/2862590/how-to-replace-master-branch-in-git-entirely-from-another-branch)
[branches](http://gistflow.com/posts/909-how-to-replace-the-master-branch-on-git)  

[Jumbo](http://en.wikipedia.org/wiki/Jumbo_frame)
[test](http://www.mylesgray.com/hardware/test-jumbo-frames-working/)
see MTU: ifconfig  
Need ICMP port open to access ping.  
http://serverfault.com/questions/234311/testing-whether-jumbo-frames-are-actually-working  

Add in the last line of a plain text file.  
```
# vim: set ts=4 sw=4 sts=4 et:
```

`dig` DNS lookup  
`set -e` ?  

(EINTR)[http://250bpm.com/blog:12]  

http://stackoverflow.com/questions/1434451/what-does-connection-reset-by-peer-mean  

python utc time: 
```
from datetime import datetime
datetime.utcnow()
```
http://stackoverflow.com/questions/15940280/utc-time-in-python  

time format output
```
time.strftime('%Y-%m-%d %H:%M:%S UTC')
```
http://stackoverflow.com/questions/3961581/in-python-how-to-display-current-time-in-readable-format  

`/usr/bin/file`: output the message of a file.  

Wrapper: ensure have the right path and enviroment.  
Output of programs should goes to /var/your-program/xxx.yaml
Put first execute file into bin. Modules into lib  

ruby enviroment for eclipse https://eclipse.org/dltk/install.php

[pgrep](http://linux.die.net/man/1/pgrep)
search processes  

[IptablesHowTo](https://help.ubuntu.com/community/IptablesHowTo)

`sudo iptables -L`

[monit](http://linux.die.net/man/1/monit)
```
monit unmonitor name
monit monitor name
```

[tcpdump](http://www.tcpdump.org/)
```
sudo tcpdump -A 
```

[openstack](http://ask.openstack.org/en/question/28335/you-should-rebuild-using-libgmp-5-to-avoid-timing-attack-vulnerability-_warnnot-using-mpz_powm_sec-you-should-rebuild-using-libgmp-5-to-avoid-timing/)
```
pip --trusted-host pypi.python.org install
```

Add a user to a group
```
useradd -G groupname username
```

[How to find]( http://stackoverflow.com/questions/6495501/find-paths-must-precede-expression-how-do-i-specify-a-recursive-search-that)

`ctrl+alt+numpad` to move the pad 

rpm: 
```
rpm -ql
```

ethtool

```
cat file | xargs
```

```
a='apple' run cmd
```
the enviroment will only exist in the cmd process. 


<code>sudo !!<code> ??? 

### VIM
```
:%s/old/new/g 
```
otherwise only on the current line

[vim search](http://vim.wikia.com/wiki/Search_and_replace>Replease and search tutorial)

```
:reg
```
to see the paste board

### SSH
##### Copy file:
With out ssh authentication:
```
nc host2 12345 &lt big-file
nc -p 12345 > big-file
```

Copy file from B to A while on B: `scp /path/file username@host:/path/destination`
Copy file from B to A while on A: `scp username@host:/path/file /path/destionation`

delete ssh-add keys:
```
ssh-add -D
```
[delete ssh key](http://stackoverflow.com/questions/25464930/how-to-remove-a-ssh-key)

SSH Forward: When ssh to another host, don't need send the keys to there to allow the new host ssh outside.  
[SSH Forward](https://w.amazon.com/index.php/EC2/Security/Howto/Setup_SSH_Credential_Forwarding)
Normal SSH:
```
ssh -i key.pem username@host
```

[ssh](http://injustfiveminutes.com/category/ssh/)
[ssh](http://ubuntuforums.org/showthread.php?t=1932058)
SSH with debug:
```
ssh -v username@host
```

### NetCat
On the listening host, i.e. on the server whose port needs to be checked, do the following:
```
nc -ul 7000
```
On the sending host, do the following - note that servname is the hostname of the listening host:
```
nc -u servname 7000
```

If text typed on the sending host (type something and hit enter) is displayed also on the listening host, then the UDP port 7000 is open.  
[netcat](http://en.wikipedia.org/wiki/Netcat)

### Python
[import module path](http://stackoverflow.com/questions/729583/getting-file-path-of-imported-module)
Compile Python:
1. config
2. sudo make -j8
3. make install

### Email
[email](http://tecadmin.net/ways-to-send-email-from-linux-command-line/)

### Networking
DNS use udp by default. when using tcp, send to many traffic.  

Switch: MAC bridge, connect devices together.   
Router: send packages.   
Internet Protocol address version 4: 32-bit number=FF.FF.FF.FF.   
IPv6:128 bits.   
CIDR: Classless internet domain routing   
DHCP: Dynamic host configuration protocol   
VIF: virtual interface. Protocol layer. Has network address.   
ASIC: application specific integrated circuit.   
RPM: RPM package manager for install software in Linux.   
Metric: The set of properties of a router.   
NAT: Network address translation   
Scope: The main feature of a product.   
Wrapper: a subroutine in a software library or a computer program whose main purpose is to call a second subroutine. a system call with little or no additional computation. To make the call of updated package much easier.   
verbose: debug or not.   
Subnet: a range of IP address.   
Security Group: a white list that allow which protocol(TCP or UDP) can access which port(e.g. SSH 22) from where(e.g. 0.0.0.0/0 or another SG). It is stateful.   
Stateless: treat every requests as independent transaction. Like HTTP.   
Stateful: create an interactive session with user. Like FTP.   
MIS: Management Information System  
Open Systems Interconnection model (OSI Model): 
1. physical layer: transmittion medium. 
2. data link layer: node to node. MAC. 
3. network layer: datagrams(variable length data sequences). Routing. IP is in internet layer.  
4. transport layer: while transmit, how to maintain quailty. TCP(on top of IP). 
5. session layer: dialogues between computers. Full/Half-duplex. 
6. presentation layer: syntax and semantics for app layer to present. 
7. application layer: show to end user. 

TCP/IP model: 
1. Link layer: how host attached. Hardware independent. 
2. Internet layer: routing, IP protocol. 
3. Transport layer: establish a basic data channel. TCP or UDP. 
4. Application layer: HTTP, FTP, SMTP, DHCP. 

IRQ: interrupt request.   
p55 latency: 55% of the targets should be faster than the given latency.  
SLA: service-level agreement. where a service is formally defined. Particular aspects of the service - scope, quality, responsibilities - are agreed between the service provider and the service user.  core dumps: record working state.  

# MTU
In IP protocol, layer 3.  
Hosts know own MTU, but don't know the smallest MTU on the path.  
IPv4 allows Fragmentation. 

The term datagram is often considered synonymous to packet but there are some nuances. The term datagram is generally reserved for packets of an unreliable service, which cannot notify the sender if delivery fails, while the term packet applies to any packet, reliable or not. Datagrams are the IP packets that provide a quick and unreliable service like UDP, and all IP packets are datagrams;[4] however, at the TCP layer what is termed a TCP segment is the sometimes necessary IP fragmentation of a datagram,[5] but those are referred to as "packets".[6]

# 计算机网络：自顶向下方法(第四版)
## 第一章
### 1.1
#### 1.1.1
Hosts connect each other through communication link and packet switch.  
ISPs follow IP protocol. 
