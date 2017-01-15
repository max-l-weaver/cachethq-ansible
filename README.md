# Deploy a Complete Cachet Server using Ansible

We are migrating our status page to Cachet and need a one click solution to deploy a Cachet server. Using Ansible
is currently the most obvious solution, although I will be migrating this to Salt shortly.

## Things to note

1. Requires Ansible 2.3 or later. This is due to an [issue with Git](https://github.com/ansible/ansible-modules-core/issues/5504)
2.The latest version of PHP Cachet runs is 7.0. They are planning on updating this at some point.
3. Tested on Ubuntu 16.04
4. When deploying your .env file, don't bother changing the mail values as these are overwritten during
the initial server setup process.