# Overview

This is a Visual Studio Code remote dev container template for doing blockchain development with node.js and Hardhat

## Note about the first run

On the very first run the container needs to be built - This can take a while. The next run will be much faster.

# How to use

Instuctions for getting started with dev containers within Visual Studio Code can be [found here](https://code.visualstudio.com/docs/remote/containers)

# Base Container

- [Ubuntu](https://github.com/microsoft/vscode-dev-containers/blob/v0.202.5/containers/ubuntu/.devcontainer/base.Dockerfile)

# Components Installed

- node.js (14.x) + npm

**Note:** You install Hardhat as a dev dependency when you create your project, it's not a globally installed tool like Truffle

# Visual Studio Code Extensions

- [Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [solidity](https://marketplace.visualstudio.com/items?itemName=JuanBlanco.solidity)

## To Initialise a new project

```
npm init --yes
npm install --save-dev hardhat

npx hardhat
```

Follow the prompts, then

```
npm install --save-dev @nomiclabs/hardhat-ethers ethers @nomiclabs/hardhat-waffle ethereum-waffle chai
```

Add the following line to the top of the `hardhat.config.js`

```
require("@nomiclabs/hardhat-waffle");
```

# Blog Post
- [Garyjackson.dev](https://www.garyjackson.dev/posts/blockchain-development-vscode-dev-containers/)
