# Example
This example provides an environment where you can test splash_auth with and OIDC auth provider of your choice.

This has been tested with podman and podman-compose. It has not been tested with docker.

##Services
### nginx
The services herin use `nginx` to handle proxying and authenticating.

### splash_auth
Provides service side support for the OIDC Code flow

### python_server
A simple python server, demonstrating that you can access it if you're logged in, and not if you're not.



## Setup
1. Edit `/examples/.env`, adding `client_id` and `client_secret` for your provider.
2. Edit `users.yml` and `api_keys.yml` adding what you need.
3. cd in to the `exmaples` directory and type `podman-compose up -d`
4. Browse to localhost:8080
 