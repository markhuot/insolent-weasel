# insolent-weasel

Insolent Weasel is a combination platter of a "data management system" and a "data storage layer". Those two pieces probably each deserve their own repo, but until then they're shoved in here.

## Data Management System

The data management system is responsible for consuming a schema from the data storage layer. That schema will create the entirety of the UI for the data management system. The data management system will POST, PUT, GET and DELETE data from the data storage layer using syntax defined in the schema, maybe through GraphQL.

A sample is saved in [data-schema.yml](data-schema.yml)

## Data storage layer

The data storage layer holds the data and responds to clients through it's schema. The data storage layer is responsible for accepting mutations and responding with structured JSON. The data storage layer can be queried by any client, not just the data management system.

A sample is saved in [ui-config.yml](ui-config.yml)
