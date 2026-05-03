# KI-101 — VPN connects but intranet unreachable

## Symptoms
- VPN connects successfully
- Internal sites (intranet) do not load
- External internet works

## Likely Causes
- DNS not updated after VPN connection
- Split tunneling policy mismatch

## Workaround (User)
1. Disconnect VPN
2. Run `ipconfig /flushdns`
3. Reconnect VPN
4. Retry intranet

## Resolution (IT)
- Verify DNS suffix search order
- Validate split tunneling configuration and routing
- If recurring, assign to Network Team

## Suggested classification
- Category: Network
- Priority: P2 (user blocked)
