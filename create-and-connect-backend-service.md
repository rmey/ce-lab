# Create and Connect Backend Service

## Create the Backend Service

1. Create the Backend Application in the Cloud Shell

```
ibmcloud code-engine application create --name backend \
--image ibmcom/backend --cluster-local --min 1
```

{% hint style="info" %}
The `--cluster-local` flag will instruct Code Engine to keep the endpoint for this application private, meaning that it will only be available from within the cluster. This is often used for security purposes. In this case, there is no reason to expose the backend application with a public endpoint, since it will not be accessed from outside of the cluster.
{% endhint %}

2. Note the backend URL and save it for later use

![](.gitbook/assets/image%20%2824%29.png)

## Connect the Frontend with the Backend Service

Execute the following command with **your** Backend URL from previous step.

```text
ibmcloud code-engine application update --name frontend \
--env BACKEND_URL=<BACKEND_PRIVATE_URL>
```

![](.gitbook/assets/image%20%2817%29.png)

