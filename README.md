# wireguard-client-connection-notification
Send a message to a Gotify server when a client is connected or disconnected from wireguard tunnel

## How to use:
- Clone this repo into your server with wireguard installed
- Rename .config-example to .config and edit the file with your Gotify host info and Gotify token.
- Make sure to add it to the root user's cron as elevated privileges are required to view the tunnel info.
- Open the terminal and type:
  - `chmod +x /path/to/wireguard-client-connection-notification/wg-clients-guardian`
  - `cp .config-example .config`
  - `sudo crontab -e`
  - `* * * * * cd /path/to/wireguard-client-connection-notification && /path/to/wireguard-client-connection-notification/wg-client-guardian /path/to/wireguard-client-connection-notification/.config`
