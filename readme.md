Directory structure and main files

LifeDAO/
├── contracts/
│ ├── LifeDAOToken.sol #ERC20Votes: Token for voting
│ ├── LifeDAOGovernor.sol # Governor: Proposal manager
│ ├── LifeDAOTreasury.sol # Treasury: Holding money and implementing proposal
│ └── LifeDAOOracle.sol # Oracle: Processing data from data provider
├── migrations/
│ └── ... # Migration scripts for Truffle
test/
│ ├── TestLifeDAOToken.js
│ ├── TestLifeDAOGovernor.js
│ ├── TestLifeDAOTreasury.js
│ └── TestLifeDAOOracle.js
backend/
│ ├── index.js # Main server file
routes/
│ tasks.js # API for task management
daos.js # API for managing DAOs
models/
taskModel.js # Model for the task
daoModel.js # Model for DAOs
dataFeedAPI.js # API that provides data for Oracle
dataProvider/
config.js # Configuration file to call and parse data from API
index.js # Clone from Klaytn's mono repo and run locally
├── package.json # Project information and dependencies
└── truffle-config.js # Truffle configuration

-------------------------------------
Description of main files and folders
contracts/: Contains smart contracts (smart contracts) written in Solidity.

migrations/: Contains migration scripts to deploy smart contracts to the blockchain network.

test/: Contains test files to ensure the smart contracts work properly.

backend/: Contains the project's backend source code.

index.js: The main file to start the server and connect to the blockchain.

routes/: Contains API management files for features like tasks and DAOs.

models/: Contains data models.

dataFeedAPI.js: API provides data to Oracle, so that Oracle can query and parse data to upload to the blockchain.

dataProvider/: Contains files related to data provider.

config.js: Configuration file to call and parse data from the backend API.

index.js: Clone from Klaytn's mono repo and run locally.

package.json: Contains information about the project and necessary dependencies.

truffle-config.js: Configuration file for Truffle.