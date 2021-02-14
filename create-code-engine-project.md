# Create Code Engine Project

1. In the IBM Cloud Shell execute the following command to create a new code engine project:

```text
ibmcloud ce project create -n <YOUR UNIQUE PROJECT NAME>
```

![](.gitbook/assets/image%20%2821%29.png)

2. Connect to the Code Engine Project using the following command

```text
ibmcloud ce project select -n <YOUR UNIQUE PROJECT NAME>
```

3. Connect the kubectl CLI to the Knative Project of Code Engine

```text
$(ibmcloud ce project current | grep export) 
```

4. Check that kubectl works

```text
kubectl get po
```

![](.gitbook/assets/image%20%2825%29.png)

{% hint style="info" %}
You have now also connected kubectl Kubernetes CLI to your Code Engine project giving you access to deeper diagnostics functions.
{% endhint %}

