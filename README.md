# Environment setup

## Skaffold config:

- install [skaffold](https://skaffold.dev/)
- verify the paths referenced on file [skaffold.yml](./skaffold.yml) file on the project directory (sibling of infra dir).
- create a jwt-secret using the command `kubectl create secret generic jwt-secret --from-literal=JWT_KEY=<your_jwt_secret_string>` - see file [auth-depl.yml](./k8s/auth-depl.yml), line 22
- navigate to this project's dir
- run `skaffold dev`
