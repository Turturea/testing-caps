# Testing Caps
This is to test if buildx still doesnt like caps in repo owners' names

## Conclusion
And it doesn't. 

## Make the pushed image private
After you make it private, you won't be able to pull it without loging in.
To log in to docker via CLI, provided you have a PAT (https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) and you exported it.
```bash
$ echo $CR_PAT | docker login ghcr.io -u Turturea --password-stdin
$ docker pull ghcr.io/turturea/buna-lume:latest
```
