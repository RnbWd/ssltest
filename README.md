# A demo Node/Express 4 app that gets A+ on the Qualys SSL Labs SSL Server Test

I'm using this app to test [letsencrypt](https://github.com/letsencrypt/letsencrypt)

## Usage

Requires **node 4.2 +**

npm install .

The following are expected:

 - Live Path `/etc/letsencrypt/live`  
 - Domain '$domain' (use your actual domain name)
 - Private key `privkey.pem`
 - Certificate `cert.pem`
 - CA certificate `chain.pem`

Start the server:

    node bin/www

Visit [Qualys SSL Labs SSL Server Test](https://www.ssllabs.com/ssltest)

Clear the cache for your site if there's an existing entry. This will initiate a new scan.

As of 2015 10 28 this Express 4 app passed the scan with A+ result.

## License

MIT

## Authors

Mike MacCana <mike@certsimple.com> @mikemaccana
