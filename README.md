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
nvm install 18
# verifies the right Node.js version is in the environment
node -v # should print `v18.20.2`
# verifies the right NPM version is in the environment
npm -v # should print `10.5.0`
# enable yarn
corepack enable
yarn -v # should print `1.22.22`

# Add to PATH
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```

## Install Hardhat

### npm

```shell
# install@latest
npm init

npm install --save-dev hardhat

npx hardhat init

# verify install
npx hardhat
```

### yarn

````shell
# install@latest
yarn init -y

yarn add --dev hardhat

yarn hardhat init

# verify install
yarn hardhat

## Hardhat Useful Command

### npm

```shell
# compile a contract
npx hardhat compile

# test a contract
npx hardhat test

# start a Local-Hardhat Network
npx hardhat node

# deploy a contract on the Hardhat Network
npx hardhat ignition deploy ./ignition/modules/Lock.js

# deploy a contract on the Local-Hardhat Network
npx hardhat ignition deploy ./ignition/modules/Lock.js --network localhost
````

### yarn

```shell
# compile a contract
yarn hardhat compile

# test a contract
npx hardhat test

# start a Local-Hardhat Network
npx hardhat node

# deploy a contract on the Hardhat Network
npx hardhat ignition deploy ./ignition/modules/Lock.js

# deploy a contract on the Local-Hardhat Network
npx hardhat ignition deploy ./ignition/modules/Lock.js --network localhost
```
