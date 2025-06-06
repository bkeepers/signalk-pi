# Signal K + Raspberry Pi setup

This is my semi-automated [Signal K](https://signalk.org/) setup on a Raspberry Pi.

## Installation

```sh
git clone https://github.com/bkeepers/signalk-pi
cd signalk-pi
bin/setup
```

## What's included

- ⛵️ [Signal K Server](https://signalk.org/) for marine data collection and distribution
- 🛢️ [InfluxDB](https://www.influxdata.com/) for persisting Signal K data
- 📈 [Grafana](https://grafana.com/) for visualizing data
- 📦 [Portainer](https://www.portainer.io/) for managing Docker containers
- 🏠 [Homepage](https://gethomepage.dev/) for a simple web interface
- ⚙️ [unattended-upgrades](https://wiki.debian.org/UnattendedUpgrades) for keeping the system up to date, and [Watchtower](https://github.com/containrrr/watchtower) for keeping docker containers up to date
- ↩️ Backup script (`bin/backup`)

<table>
<tr>
<td><img alt="Homepage" src="https://github.com/user-attachments/assets/c1ca5441-a152-410e-9221-2dfa01f05dcb" /></td>
<td><img alt="Signal K" src="https://github.com/user-attachments/assets/b5fffa47-bb95-4f32-b978-381f92fd4a33" /></td>
</tr>
<tr>
<td><img alt="Grafana" src="https://github.com/user-attachments/assets/f91cb05c-85ac-4af9-9e8a-55c00fd2be57" /></td>
<td><img alt="Portainer" src="https://github.com/user-attachments/assets/b0a6f1dc-9f3a-4137-8a57-8a7180d0f0a5"/></td>
</tr>
</table>

## To Do

- Auto-create access point when no network is available
- One-line install script (`curl … | bash`)
- Automate grafana configuration
- Automate running `bin/update` periodically
- Automate running `bin/backup` periodically
- `bin/restore` to restore one or more services
