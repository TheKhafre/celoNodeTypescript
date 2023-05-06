## clone the celo monorepo to your machine with this command
    git clone github.com/celo-org/celo-monorepo.git

## To initialize the project, run the npm initialization command below
	npm init -y

## Install the TypeScript packages as a development dependency. To do this, use the command:
	npm install typescript --save-dev

## install dependencies with this command from the monorepo directory
    yarn install

## build the new packages by running
	yarn build –ignore docs

## Generate Validator Key
    yarn run generate:validator

## Create configuration file by copying the template into a new file named .env file with the command
    cp .env.template .env

### the file should contain the following lines which should be adjusted accordingly:
    CELO_VALIDATOR_ADDRESS=<your-validator-address>
	CELO_VALIDATOR_PRIVATE_KEY=<your-validator-private-key>
	CELO_BOOTNODES=<comma-separated-list-of-bootnodes>

## Start the node by running the command
    yarn run start:fullnode

## Monitoring the node
### to view the node status, run command:
    yarn run celo status
### to view log:
    yarn run celo logs