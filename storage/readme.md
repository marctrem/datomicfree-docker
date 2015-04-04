Build the storage container image
`docker build -t marctrem/datomic-data-img .`

Create a named container
`docker create -v /datomic-data --name datomic-data marctrem/datomic-data-img`

