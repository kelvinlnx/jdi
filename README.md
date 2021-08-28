# jdi
README
======
To do everything, just run the jdi command

This project assumes:

	- Host OS is Ubuntu 20.04
	- Firewall on Host OS is enabled - ufw (playbook sage.yaml uses it)	  # to be verified, what happens if not enabled?
	- ansible is installed
	- cgroup-tools is installed (only if memory profile required)
	- python3-lxml is installed

This project uses:

	- Host machines libvirt "default" network

IMPORTANT:

	1. make sure you modify the all-vars file in vars directory before running jdi
	2. make sure you modify the cloud-config settings (line 86) in sage.yaml,
	   edit genrepo.yaml and set cleanmeup to true to cleanup files after install.
	3. run: ./jdi --help
	4. run installer: jdi
