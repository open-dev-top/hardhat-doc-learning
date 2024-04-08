# hardhat-doc-learning

[Getting started with Hardhat](https://hardhat.org/hardhat-runner/docs/getting-started#overview)

## [Install WSL2](https://learn.microsoft.com/en-us/windows/wsl/install)
```shell
wsl -- install
```

## [Install Node.js](https://nodejs.org/en/download/package-manager)
```shell
# installs NVM (Node Version Manager)
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash

# download and install Node.js
nvm install 20

# verifies the right Node.js version is in the environment
node -v # should print `v20.12.1`

# verifies the right NPM version is in the environment
npm -v # should print `10.5.0`

# Add to PATH

```
export NVM_DIR="$HOME/.nvm"

[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm

[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
