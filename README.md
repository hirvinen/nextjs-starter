# A Next.js starter project

This is a starter project to serve as a template for Next.js applications.

It is not a clone of, but inspired by [Next.js Starter Project](https://github.com/iaincollins/nextjs-starter) by [Iain Collins](https://github.com/iaincollins) . It will probably do many things in a similar fashion, while others may reflect different preferences. The main reason for doing this myself is to learn more about what's going on under the hood.

## Features / objectives

See TODO.md for what is yet to be implemented

* Authentication
  * Email, Facebook, Twitter, Google+ etc.
  * 2FA
  * Passwordless logins
* User accounts
  * Basic account management
  * Basic group based access levels
* Security
  * Session support with secure HTTP Only cookies
  * CSRF Tokens
  * CSP
  * HTTPS only by default
    * In production, there is no place for HTTP.
    * If serving content directly to the public, point your config to a proper certificate.
    * A more ready-to-scale solution would be to start with e.g. nginx as a reverse proxy, using proper certificates, and have application instances use snakeoil certificates for HTTPS between proxy and application instances.
    * Optionally only allow requests from proxy with client certificates.
    * HSTS
