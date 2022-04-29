# vagrant-ansible-confluence-postgres

You might want to change the following values to adapt it with your hardware.

```
    v.memory = 8096
    v.cpus = 8
```

Modify Confluence version on play.yml and confluence.service (change 7.13.4 for the version you want to install).

Once saved, execute `vagrant up`. When vagrant images are up, access to http://192.168.56.11:8090/ to proceed with Confluence installation.

After setting up the mode (Trial or Production) the license and the deployment type (Standalone or Clustered), you have to setup the DB.

Select the following:

```
Database type: PostgreSQL

Setup type: By connection string

Database URL: jdbc:postgresql://192.168.56.10:5432/confluence

Username: confluence

Password: confluence
```
