<img src="https://www.fastly.com/altitude/assets/logo-7d39dce955f0bcb44b1c3b53871b2f9af80b843979c8188fc7f5e0feb782b768.png" width="300">

# Building a continuous deployment pipeline 
This repository contains the files and excercises needed to participate in the [Fastly Altitude SF 2017](https://www.fastly.com/altitude/) workshop "Building a continuous deployment pipeline".

**Welcome!**
The goal of the workshop is to build a continuous deployment pipeline around an example Fastly config. Combining Fastly’s 5-second deploys, API control, and some open-source tooling ([Travis](https://travis-ci.org/), [Terraform](https://www.terraform.io/)) attendees will contribute live changes and see their results in the demo.

## Prerequisites
- Have a GitHub account
- Have a machine with a terminal prompt, `Make` and `Ruby` installed (*not required if using provided workstation)

## Install:
Altitude attendees will be provided with a pre-provisioned server with all software and files needed already installed for you convienince. The conncetion details will be handed out to you.
- [Create a new GitHub repository](https://help.github.com/articles/create-a-repo/), called `altitude-ci-cd-workshop`.
- `ssh -A altitude@<IP of host assigned to you>`
- `cd workshop`
- `git remote add origin git@github.com:<USERNAME>/altitude-ci-cd-workshop.git`

Alternatively if you aretrying this at home:
- Fork the GitHub repo: [https://github.com/fastly/altitude-ci-cd-workshop](https://github.com/fastly/altitude-ci-cd-workshop)
- Clone the repo to a local directory on your machine:
    - Via SSH: `git clone git@github.com:<USERNAME>/altitude-ci-cd-workshop.git`
    - Via HTTP: `git clone https://github.com/<USERNAME>/altitude-ci-cd-workshop.git`
- Change directory into the repo: `cd altitude-ci-cd-workshop`
- Install the dependencies `make install`
    - This will install the Terraform binary to your `$HOME` directory and link your `$PATH`. Permission may be required.
    -  If you already have [Terraform](https://www.terraform.io/downloads.html) and the [Travis gem](https://github.com/travis-ci/travis.rb#installation) installed on your machine or would prefer to install manually, skip this step.
- You're good to go!

## Exercises:
To start, follow the tasks in the `exercises` directory:

1. [Define a Fastly service with Terraform](exercises/1.md)
2. [Configure continuous deployment with Travis](exercises/2.md)
3. [Setup multiple environments: staging & production](exercises/3.md)
