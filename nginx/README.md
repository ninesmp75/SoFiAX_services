# nginx

Reverse proxy server for deploying services through docker compose.

## Configuration

There are a number of steps necessary to set up your SSL certificate on the `nginx` server. This will be necessary for clients to connect securely to the site. 

The steps are:

1. Identify a certificate authority to use
2. Purchase SSL certificate
3. Domain ownership verification (multiple methods for doing this - we have used HTTP file authentication).
4. Configure `nginx/default.conf` 
5. Redeploy services

Here are some resources on how to do this

* https://certpanel.com/comodo/client/orders.aspx (purchase SSL certificate)
* https://phoenixnap.com/kb/install-ssl-certificate-nginx