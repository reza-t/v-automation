# v-automation

## Steps to run install the platform

### checkout the ip address is valod

```bash startNginx.sh```

### install the v2ray platform
if the ip address is accessable in you country move to next steps.

The `install.sh` will be uninstall the nginx first and then install the platform. 

 ```bash install.sh <3x-ui version> <username> <password> <port>```

Example: 
`bash install.sh v1.7.9 y root 123456778 8443`

if you skip passing the parameters during the installation you will get prompt to enter the parameters.

### Setup Config

login to the platform by navigating to the <ipaddress>:8443 and copy the config from the `xray-configuration-template.json` to the `/Panel Settings/Xray Configuration/Complete Template`.

### Create the Inbound

Configure the Inbound and here is some example:

- protocol: `vless`
- port:`8080` or `443`
- Turn on `Reality`
- Transmission: `TCP`
- Dest: `www.speedtest.net:443`
- Server Names: `www.speedtest.net, speedtest.net`

Click on `Get New Key`