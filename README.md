# Kubernetes Jump Host Setup

## Overview

This Bash script automates the setup of all Kubernetes(AKS) in a determined Azure Subscription using Jump Host.
The script stores those in a screen session, avoiding needing to open a new terminal window(which is something that I dislike)

- Required tools (`az`, `jq`, `screen`, `kubectl`)

## Prerequisites

Before running this script, ensure you have the following tools installed:

- Azure CLI (`az`)
- `jq`
- `screen`
- `fzf`
- `kubectl`

## Usage

1. Set the environment variable `JUMPHOST_FQDN` as `export JUMPHOST_FQDN="someservername.somedomain.com"
2. Run the script in your terminal.
3. Follow the prompts to select your Azure subscription.
4. Sit back and let the script set up the Kubernetes Jump Host for you.

### Note

To make the actual screen sessions available in your terminal, you will need to run the following commands after the script has completed:

```bash
export SCREENDIR=$HOME/.screen
export KUBECONFIG=$HOME/.kube/config
```


Now, go ahead and use this script with confidence, knowing that it's been carefully handcrafted by your friendly neighborhood human coder(and that is true). 😉
