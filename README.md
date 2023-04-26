## clone the celo monorepo to your machine with this command
    git clone github.com/celo-org/celo-monorepo.git

## install dependencies with this command from the monorepo directory
    yarn install

## Generate Validator Key
    `yarn run generate:validator`

## Create configuration file by copying the template into .env file with the command
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