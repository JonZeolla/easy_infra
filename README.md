<h1 align="center">Easy Infra[structure as Code]</h1>

easy_infra is a docker container that simplifies Infrastructure as Code deployments.

## Quickstart
### Ansible
1. To run an ansible playbook run the container, volume mount the playbook, and provide the required arguments to get passed to `ansible-playbook`:
```
docker run -v $(pwd)/key:/root/keys/key -v $(pwd):/root/ansible seiso/easy_infra:latest -u user -i 192.0.2.230 --private-key /root/keys/key /root/ansible/playbook.yml
```

## Contributing
1. [Fork the repository](https://github.com/SeisoLLC/easy_infra/fork)
1. Create a feature branch via `git checkout -b feature/description`
1. Make your changes
1. Commit your changes via `git commit -am 'Summarize the changes here'`
1. Create a new pull request ([how-to](https://help.github.com/articles/creating-a-pull-request/))

