# Google Cloud Platform
In order to run distributed versions on the cloud, launch the scripts in sequence.
- decide the hyperparameters by setting environment variables in 00.variables.sh
- create bucket on Google Cloud Storage
- load data to the just created bucket
- you can decide whether to run a single-node cluster (3b.dataproc-create-single-node.sh)
or to run a multi-worker cluster (first run 3a.dataproc-create-cluster.sh to get a 2-workers cluster, if you want to start with a bigger cluster size, accordingly set DATAPROC_NUMWORKER variable and then run 05.dataproc-scaleup.sh before submitting a job)
- submit a Scala+Spark job
- scale up the multi-worker cluster size
- down scale the multi-worker cluster size
- deallocate Dataproc resources
- deallocate Google Cloud Storage resources.
