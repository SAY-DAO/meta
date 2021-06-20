### Create SSL for any site

1. Install certbot if needed: https://certbot.eff.org/lets-encrypt

2. Run this command as root in the server and follow the instruction:

```bash
certbot certonly --manual -m 'it@say.company' -d say.company -d *.say.company --preferred-challenges dns --agree-tos
```
3. Use in cpanel:
    - `/etc/letsencrypt/live/say.company/privkey.pem` as KEY
    - `/etc/letsencrypt/live/say.company/cert.pem` as CRT
    - `/etc/letsencrypt/live/say.company/chain.pem` as CABUNDLE

## NOTE
`say.company` is an example and placeholder, you can change it to any domain. **BE CAREFUL to change every occurance.**
