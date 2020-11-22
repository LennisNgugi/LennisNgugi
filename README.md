<!-- Zero width character is used to put extra blank lines before and after code -->

<h3>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple = ("Python", "Bash", "HTML/CSS", "SQL", "Swift", "C#")
    databases   : tuple = ("SQL Server 2017", "PostgreSQL", "Mongo")
    ongoing     : tuple = ("Django", "GraphQL", "JavaScript", "Rest APIs", "Soap APIs")
    reconnaissance  : tuple = ("Nmap", "Netdiscover", "Aircrack-ng", "Shodan", "Metasploit Framework")
    reverse engineering : tuple = ("Ghidra")
    forensics : tuple = ("AccessData (FTK) Imager", "AccessData (PRTK)", "AccessData Registry Viewer", "iPhone-backup-analyzer")
    sniffing & spoofing : tuple = ("Wireshark", "Bettercap", "SET", "Burp Suite", "Wifi Honey")
    password : tuple = ("John the Ripper", "Johnny", "Hydra", "Wordlists", "Ophcrack")
    operating systems : tuple = ("Kali linux", "Mac", "Windows")
    

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```
</h3>
