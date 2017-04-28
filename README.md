# Azure SNACK

Creates a Kubernetes Cluster on Azure with Spark, Cassandra, Kafka, PostGIS, and Deis Workflow.

To use:

1. Install the Azure 'az' CLI tool.
2. Find your Azure subscription ID.  Make sure 'az' is logged into this subscription by doing a 'az account list' and confirming this subscription is in the list.
3. Choose a deployment prefix.  This is basically a name that uniquely identifies your cluster.  (eg. 'mycluster')

$ cd ops

$ SUBSCRIPTION_ID="04f7ec88-8e28-dead-beef-5e17766001f5" DEPLOYMENT_PREFIX="mycluster" ./create-snack-cluster
