# Stuff that needs doing

* Pretty much everything in README.md

## Possibly useful libraries

* [passport-client-cert](https://www.npmjs.com/package/passport-client-cert) for only accepting requests from proxies

## Notes on using LE certificates

* When using a reverse proxy in front of the application, the certificate for the public-facing hostname must be available to the proxy.
* However, the proxy needs to let through the ACME challenges for obtaining a certificate for the backend server, to use LE certs for that, instead of snakeoil certs.
* TODO: Add example nginx config for this?
