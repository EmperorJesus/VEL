Connection &amp; functions for connection between IoT device and BDB testnet.
Examples and functions for connection, registration, and updating of IoT device info & readouts with BDB.
Web interface coming soon. Bash script for uploading and hosting via GitHub Pages.

Sequelize being used for Postgres ORM. Users stored in this db to get around worries re: setting up our own blockchain-based ID system + GDPR compliance..

*see* `./details.txt` *for further info*

- [ ] need append tx in `python/automated_sensehat_upload`
- [x] change connection in `python/automated_sensehat_upload` to tesnet
- [x] consolidate `prep_code/javascript_prep` into just connection + functions
- [x] db setup for standard users
	+ [x] routes
	+ [x] db models
	+ [x] config
- [ ] create web interface (hosted via GitHub Pages or Netlify):
	+ [x] html skeleton
	+ [ ] uPort login / integration
	+ [ ] 'standard' login
		- [ ] db orm interfacing
		- [ ] cookie + secret
		- [ ] secure signup (bcrypt)
	+ [ ] http(/s) for all functions in drivers:
		- [ ] registerDevice()
		- [ ] deviceInfo()
		- [ ] update()
		- [ ] burn()
	+ [ ] infographics (scrape BDB)
	+ [x] .sh for upload & hosting

Further *potential* development paths
- [ ] integrate FOAM for geo-spatial data verification ( cf. https://f-o-a-m.github.io/foam.developer/ for tools)
- [ ] look into classification of 'data trustworthy-ness' re: method of data input
	+ [ ] look into potential to build atop this re: levels of trusted data (e.g. TCR)
