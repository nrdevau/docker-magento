<h1 align="center">nrdevau/docker-magento</h1>

<div align="center">
  <p>Nate's docker Magento 2 setup - heavily inspired by Mark Shust's Docker Configuration for Magento</p>
</div>

## Table of contents

- [Usage](#usage)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Updates](#updates)
- [Custom CLI Commands](#custom-cli-commands)
- [Credits](#credits)
- [License](#license)


## Usage

This configuration is intended to be used as a Docker-based development environment for Magento 2.

This will clash with apache or NGINX running on your host. Please disable those services or change the port in the config
Copy files out of compose to local directory
Run 
```
bin/download 2.4.6-p2 community # <or your version>
# Run the setup installer for Magento:
bin/setup magento2.nrdev.local

open https://magento2.nrdev.local
```

Needed to change the PHPMyAdmin port in the compose.dev.yaml file
Login to admin portal with credentials in bin/setup-install
Check mail caught using mailcatcher http://magento2.nrdev.local:1080/ - to setup 2FA