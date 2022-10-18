# Blockchain Dashboard 

This repository contains the sample data format for blockchain interoperability dashboard project.

Data Sources: 
- https://www.livecoinwatch.com/
    - Contains market data for token based projects

- https://messari.io/
    - (Sometimes) Contains infomration about user activity

Data format:

The data from the backend will be served to the webpage in a json list. 
Each item in this list represents data about an interoperability project.
More fields can be added in the future. 
For project-specific attributes, (e.g. Polkadot or Cosmos's # validators) the 'Extra' field must be used. 

```json
"ProjectName": "Polkadot",
"ActiveAddressCount": 22000,
"CirculationSupply":12430000,
"TotalSupply": 11540000,
"Explorer": "https://explorer.polkascan.io/",
"Extra": {
    "something": "project specific information should be stored here"
}

```