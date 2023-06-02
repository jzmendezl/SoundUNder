# SoundUNder_rps

## Prerequisites
Have both Docker and Docker compose plugin installed in the machine.

## How to Run the Proxies

To run the reverse proxies, follow these steps:

1. Clone the GitHub repository to the desired machines.
2. Open a terminal and navigate to the root directory of the project.
3. Download the **certs** folder from the .Envs shared drive folder.
4. Go to the **app.conf** files inside each folder and change the desired IP and ports on the second line of the files.
5. Once all the needed changes are done, run the following command (remove the -d if you want to see the logs in the console):
``` console
docker compose up -d
```

## How to Use the Reverse Proxies

The ports specified in the docker-compose file must be exposed in the machine where the rps will be running. Then, to access them simply put the machine's public ip or the domain name linked to it and the port of a rp.