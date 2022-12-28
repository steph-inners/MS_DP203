# Azure for the Data Engineer
[Azure for the Data Engineer](https://docs.microsoft.com/en-us/learn/paths/azure-for-the-data-engineer/)

Data abundance
- increase in software and devices that generate data
- increase in human consumers of data and how they view it
- structured and unstructured

On-prem vs cloud data
- on prem
	- physical PC cost, OS licensing, hardware software firmware maintenance
	- scale by adding more nodes and clustering with load balancing
		- in clustering, each server in the cluster must be identical
	- availability / uptime
		- 3 nines, 4 nines or 5 nines
		- multiply by hours in year (8760) to see hourly up/down time
	- on-prem multilingual support is expensive
		- sort order requires reconfig, only an option if DBAs designed system to support multilingual
	- TCO (total cost of ownership) for on-prem includes
		- hardware
		- software
		- labor
		- datacenter overhead (power, telecom, cooling, etc)
	- if demand increases, need to immediately purchase new equipment
		- cost often capitalized (spread out across expected server lifespan) so hard to argue for more earlier
- cloud
	- charged as monthly sub, so no capitalizing across server lifespan
	- scalability by compute units, defined differently per Azure product
		- cost more closely matches usage
	- economies of scale bring lower costs
	- development environments are cheaper than prod
	- **lift and shift** strategy moves from on-prem to cloud without rearchitecting the app
		- quick and easy
		- but doesn't take advantage of all Azure features
	- unstructured data schema is typically defined at query time
		
Understand job responsibilities
- focus shifts away from SQL Server and toward general data, as a data engineer
- data engineers work with unstructured and variety of data, as well as relational data
- may need to learn new tools and languages
- ETL
	- transformation can take a long time
	- ties up resources
	- traditionally moves data from on-prem to on-prem
- ELT
	- data immediately extracted and loaded
	- more flexibility for multiple transformations for different uses
	- typically used for data from on-prem to cloud
- shift focus away from server implementation
	- simpler deployments if you want
	
Use cases for the cloud
- support web apps with quick response times anywhere in the world
- easily collab with data scientists using R, Scala, Python, etc.
- some Azure products designed specifically for IoT

NEXT: https://learn.microsoft.com/en-us/training/modules/evolving-world-of-data/1-introduction