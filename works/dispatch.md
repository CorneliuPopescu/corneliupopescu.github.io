# Dispatch by Netflix

## [Installation](https://hawkins.gitbook.io/dispatch/installation)

### PoC

**Installing Dispatch from Docker**

See [installation instructions](https://hawkins.gitbook.io/dispatch/installation)

- Requirements
  - Windows 11 workstation
    - WSL2
    - Docker Desktop
    - Docker Compose
- Actions

```bash
git clone https://github.com/Netflix/dispatch-docker.git
# copy .env.example file to a new .env file and set proper secrets
sudo ./install.sh
# Load example data? yes
sudo docker-compose up -d
# http://localhost:8000/default/auth/register
# corneliu@p1.cl
sudo docker exec -it dispatch_web_1 bash -c 'dispatch user update --role Owner --organization default corneliu@p1.cl'
# User successfully updated.
```

## Resources

- [Introducing Dispatch](https://netflixtechblog.com/introducing-dispatch-da4b8a2a8072)
- [Dispatch - GitHub repo](https://github.com/Netflix/dispatch)
- [Dispatch - Docs](https://hawkins.gitbook.io/dispatch/)
