# Use IBM Cloud Object Storage for the Backend

## Create an new IBM Cloud Object Storage Bucket

In the Cloud Account we have a predefined IBM Cloud Object Storage Instance which support S3 API which we will utilise to store text files to be analysed. In this instance we create a **unique bucket** using the following command in the Cloud shell. Please use small capitals to create a uniques bucket name, see screenshot.

```
ibmcloud cos bucket-create \
--ibm-service-instance-id crn:v1:bluemix:public:cloud-object-storage:global:a/e97a8c01ac694e308ef3ad77957bb960:1ef3fc71-c501-4369-be8b-dfe99c0c7954:: \
--class Standard --region eu-geo --bucket <YOURUNIQUEBUCKETNAME>
```

![](.gitbook/assets/image%20%2812%29.png)

## Connect the COS Service with the Backend

{% code title="hello.sh" %}
```bash
# Ain't no code for that yet, sorry
echo 'You got to trust me on this, I saved the world'
```
{% endcode %}



