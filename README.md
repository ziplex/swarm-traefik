# swarm-traefik

This is a **sample** traefik proxy swarm deploymen topology.

Please;
- Update "domain" in "proxy.toml"
- Add your certifacates under "./tls/cert.pem", "./tls/key.pem"
- Or use "setup-cert.sh" to generate them

- Create a network for traefik
```bash
docker network create -d overlay proxy-net
```
- Then run 
```bash
docker stack deploy -c docker-compose.traefik.yml traefik
```
