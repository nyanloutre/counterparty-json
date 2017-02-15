# Contient les JSON de mes différents assets

## PEPELEO

http://blockscan.com/assetInfo/PEPELEO

# Utilisation

```
docker run -d --name=counterparty-json \
    --label traefik.frontend.rule=Host:json.nyanlout.re \
    --label traefik.port=80 \
    -v /srv/counterparty-json:/usr/share/nginx/html:ro \
    --network nginx-net \
    --restart always \
    nginx:alpine
```
