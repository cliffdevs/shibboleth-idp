# Shibboleth-IDP for Docker
This repository contains a customized shibboleth-idp dockerfile to build a custom image. It has default configurations and a self-signed certificate for the embedded web service with all passwords set as the default 'changeme'. This is not intended for use in any live environment, but only for local testing and learning excercises. 

To build this, clone the repo and execute
```shell
docker build -f shibboleth-idp.dockerfile -t <yourcompany>/shibboleth-idp:<desiredversion> .
```

To run it
```shell
docker run -it -p 443:443 <yourcompany>/shibboleth-idp:<desiredversion>
```
