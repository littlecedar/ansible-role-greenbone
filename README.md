# ansible-role-greenbone

Adopts an existing Greenbone Community Edition Compose stack.

- Compose project: `greenbone-community-edition`
- Default path: `/opt/siem/greenbone`
- HTTPS on host port 9443
- Daily feed sync at 03:15 (`greenbone-feed-sync.timer`), including a dangling-image prune
- Copies `compose.yaml` only when the host does not already have one
- Does not delete volumes

`greenbone_enabled` defaults to false.
