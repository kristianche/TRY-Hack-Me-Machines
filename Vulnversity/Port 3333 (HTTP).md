# Directory Brute Forcing

I have fuzzed the http port using the tool: **FUZZ**

```json
ffuf -u http://10.10.155.145:3333/FUZZ -w /usr/share/wordlists/dirb/common.txt
```

![[Pasted image 20250807130720.png]]

# File Upload Vulnerability

The */internal/* path is vulnerable to **File Upload**

![[Pasted image 20250807130951.png]]


