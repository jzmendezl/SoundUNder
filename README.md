#SoundUNder

### Run
Change branch git
```sh
git submodule foreach git checkout deploy_vm
```

Clone the repository and run the following command to get the submodules:

```sh
git submodule update --init --recursive
```

Then run the following command to start the project:

```sh
docker-compose up -d --build
```
