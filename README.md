Run Jenkins in Docker command (and pass Docker socket)

```bash
docker run -u root -d --name blue-ocean -p 8080:8080 -v jenkins-data:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock jenkinsci/blueocean:latest
```

- all data is stored in Docker volume "jenkins-data"
- see password with `docker logs blue-ocean`
- user `tester`
