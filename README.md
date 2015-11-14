# Let’s Encrypt A+ SSL Server Test

A zero-config Node/Express 4 app that gets A+ on the Qualys SSL Labs SSL Server Test

First install [letsencrypt](https://github.com/letsencrypt/letsencrypt) and generate some *real certs*. Documentation can be found [here](https://letsencrypt.readthedocs.org/en/latest/index.html).

## Usage

Requires **node 4.2.x**

npm install .

The following are expected:

 - Live Path `/etc/letsencrypt/live/${domain}` 
 - Private key `privkey.pem`
 - Certificate `cert.pem`
 - CA certificate `chain.pem`

Start the server:

    node bin/www

Visit [Qualys SSL Labs SSL Server Test](https://www.ssllabs.com/ssltest)

Clear the cache for your site if there's an existing entry. This will initiate a new scan.

As of 2015 11 14 this app passed the scan with A+ result.

Much love [Let's Encrypt](https://letsencrypt.org)

## License

MIT
