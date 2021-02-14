# Create and test the Watson Text Analyser Job

In our final chapter of the Tutorial we would like to create the Code Engine Job which analyses the uploaded text files with the IBM Cloud [Watson Natural Language Understanding](https://www.ibm.com/cloud/watson-natural-language-understanding) Service \(NLU\).

## Create an Watson NLU API Key

```text
ibmcloud resource service-key-create <YOUR-UNIQUE-NLU-KEY-NAME> Manager --instance-name code-engine-nlu
```

![](.gitbook/assets/image%20%2824%29.png)

## Create a Secret for COS and Watson NLU Services for the Backend Job

Adopt the following command in your editor of choice with your COS **bucket name** and **COS** **API key** \(from previous chapter\) and the **Watson NLU API Key** and execute in Cloud Shell, this will create a file nlu.env.

```text
cat << 'EOF' > nlu.env
NLU_JOB_APIKEY=<YOUR NLU API KEY>
NLU_JOB_URL=https://api.eu-de.natural-language-understanding.watson.cloud.ibm.com/instances/f4c4e4d9-f8dc-49fe-b7b3-15f6fcf44d51
COS_ENDPOINT=https://s3.eu.cloud-object-storage.appdomain.cloud
COS_JOB_APIKEY=<YOUR COS API Key>
COS_JOB_RESOURCE_INSTANCE_ID=crn:v1:bluemix:public:cloud-object-storage:global:a/e97a8c01ac694e308ef3ad77957bb960:1ef3fc71-c501-4369-be8b-dfe99c0c7954::
COS_BUCKETNAME=<YOUR BUCKET NAME>
EOF
```



