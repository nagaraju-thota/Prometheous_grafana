# Docker Commands

## Pull Image

```bash
docker pull prom/prometheus
Run Container
docker run -d --name prometheus -p 9090:9090 prom/prometheus
List Containers
docker ps
Stop
docker stop prometheus
Start
docker start prometheus
Restart
docker restart prometheus
Logs
docker logs prometheus
Live Logs
docker logs -f prometheus
Remove
docker rm -f prometheus

---