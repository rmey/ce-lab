# Create and test the Watson Text Analyser Job

In our final chapter of the Tutorial we would like to create the Code Engine Job which analyses the uploaded text files with the IBM Cloud [Watson Natural Language Understanding](https://www.ibm.com/cloud/watson-natural-language-understanding) Service \(NLU\).

## Create an Watson NLU API Key

```text
ibmcloud resource service-key-create <YOUR-UNIQUE-NLU-KEY-NAME> Manager --instance-name code-engine-nlu
```

![](.gitbook/assets/image%20%2824%29.png)

## Create a Secret for COS and NLU for the Backend Job



