Build the transactor container image


`docker build -t marctrem/datomic-transactor .`



Create a transient container

`docker run -it --rm --volumes-from datomic-data --name transactor marctrem/datomic-transactor`

