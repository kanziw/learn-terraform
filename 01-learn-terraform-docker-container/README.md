# learn-terraform-docker-container

> https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/aws-get-started#quick-start-tutorial


Initialize the project, which downloads a plugin that allows Terraform to interact with Docker.

```zsh
$ terraform init
```


Provision the NGINX server container with `apply`. When Terraform asks you to confirm type `yes` and press `ENTER`.
```zsh
$ terraform apply
```


Verify the existence of the NGINX container by visiting localhost:8000 in your web browser or running docker ps to see the container.

```zsh
$ docker ps
CONTAINER ID   IMAGE          COMMAND                  CREATED         STATUS         PORTS                               NAMES
d6ade8820b02   0c404972e130   "/docker-entrypoint.…"   6 seconds ago   Up 5 seconds   0.0.0.0:8000->80/tcp                tutorial
```
