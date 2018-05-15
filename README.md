# DevOps Crash Course

In this lab, we will try some of the tools in the DevOps tool chain to (i) provision VMs, (ii) manage configuration, (iii) deploy our app.

Specifically, we'll cover the following tools:
- shell
- configuration management: ansible
- cloud resources provider: Google Cloud Platform

At the end of course we will deploy our node.js app onto vanilla (i.e. fresh) VMs (i.e. computers). Along the way, we will apply Infrastructure as Code / DevOps practices around (i) automated provisioning and (ii) automated configuration management

### Setup
- Create GCP account @ https://cloud.google.com/
- 


### Outline
- Bare hands
  - provision VM on GCP Google Compute Engine
  - ssh into GCP VM
    - `ssh -i ~/.ssh/id_rsa.pub`
  - Running shell commands by hand on VMs
    - git: `sudo apt-get install git`
    - nodejs:
      - `curl -sL https://deb.nodesource.com/setup_9.x | sudo -E bash -`
      - `sudo apt-get install -y nodejs`
    - yarn: 
      - `curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -`
      - `echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list`
      - `sudo apt-get update && sudo apt-get install yarn`
  - Get source code
    - git clone 
  - Open firewall
    - 
  - Start application: `yarn start`

- Ansible
  - Repeat all of the above in ansible
  - 