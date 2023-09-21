 run this command to configure the runner:

```bash
docker-compose up -d
docker-compose exec gitlab-runner gitlab-runner register
```
for running dind you need setup following config
    privileged = true
    volumes = ["/cache", "/var/run/docker.sock:/var/run/docker.sock"]
