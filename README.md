# docker compose file for Grafana service with SSL connection

to start the container:
* sudo socker compose up -d 

## Before stating up the container, you must set the environment variables: 
* GF_SERVER_DOMAIN 
* GF_SECURITY_ADMIN_PASSWORD
* GF_AUTH_GENERIC_OAUTH_CLIENT_ID
* GF_AUTH_GENERIC_OAUTH_CLIENT_SECRET

  
To obtain the GF OAUTH CLIENT ID and CLIENT SECRET configure your application in https://iam.cloud.infn.it/.


You must also have a fullchain.pem and a privkey.pem (req -x509 -sha256 -nodes -days 365 -newkey rsa:2048 -keyout privateKey.key -out certificate.crt) 
