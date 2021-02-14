# Create Frontend Application

## Create the Frontend Application using the CLI

1. Execute the following Command in the Cloud Shell

```
ibmcloud code-engine application create \
--name frontend --image ibmcom/frontend --min 1 
```

![](.gitbook/assets/image%20%2814%29.png)

2. Open the URL of the Frontend Applikation in a new Browser Tab

![](.gitbook/assets/image%20%2822%29.png)

## Optional - Scale the Frontend Application

Enter the following commands to scale the application and get details of the application.

```text
 ibmcloud code-engine application update --name frontend --max-scale 3
 ibmcloud code-engine application get -n frontend
```

![](.gitbook/assets/image%20%2817%29.png)

