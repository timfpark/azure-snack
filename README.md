# Azure SNACK

Creates a Kubernetes Cluster on Azure with Spark, Cassandra, Kafka, PostGIS, and Deis Workflow.

To use:

1. Install the Azure 'az' CLI tool.
2. Find your Azure subscription ID.  Make sure 'az' is logged into this subscription by doing a 'az account list' and confirming this subscription is in the list.
3. Add the public ssh key for the identity that you'd like to connect with in the 'ssh' directory and call it 'id_rsa.pub'.
4. Choose a deployment prefix.  This is basically a name that uniquely identifies your cluster.  (eg. 'mycluster')
5. Adjust any of the default values in create-snack-cluster to meet your needs.  You can also comment out any of the pieces of infrastructure that you don't need.
6. Run the script:

```
$ cd ops
$ SUBSCRIPTION_ID="04f7ec88-8e28-dead-beef-5e17766001f5" DEPLOYMENT_PREFIX="mycluster" ./create-snack-cluster
```
