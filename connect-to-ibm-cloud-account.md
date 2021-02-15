# Connect to IBM Cloud Account for Workshop

### Prerequisites

* existing IBM ID and trial or paid IBM Cloud account
* modern Browser like Chrome, Firefox
* Internet connectivity

### Connect IBM Cloud Account

1. Goto to [https://cloud.ibm.com/login](https://cloud.ibm.com/login) and login to your IBM Cloud Account using your IBM ID 
2. Open the following URL in a new browser tab and enter your IBM ID and the Workshop **Password** given by the instructor: [https://ce-workshop-dach.eu-de.mybluemix.net](https://ce-workshop-dach.eu-de.mybluemix.net/) and press submit.  

![](.gitbook/assets/image%20%286%29.png)



3. Now you should see the following confirmation. Follow the first link from the Dialog or use that link: [https://cloud.ibm.com/resources?bss\_account=e97a8c01ac694e308ef3ad77957bb960](https://cloud.ibm.com/resources?bss_account=e97a8c01ac694e308ef3ad77957bb960)

![](.gitbook/assets/image%20%289%29.png)

### Accessing the IBM Cloud Account/Cloud Shell

You should now connected to the following IBM Cloud Account:

![Check upper right area that your are in that Account shown.](.gitbook/assets/image%20%282%29.png)

1. Open Code Engine Project View \(navigation from the hamburger menu to resource list code engine project\)

![](.gitbook/assets/image%20%284%29.png)

![](.gitbook/assets/image%20%288%29.png)

2. Open a IBM Cloud Shell Window, this will start our Terminal in the Browser, we use for exercises and commands, we don't need a local CLI.

![](.gitbook/assets/image%20%287%29.png)

3. The Cloud Shell will open in a new Browser Tab. Choose Location Frankfurt in the upper right menu  


![](.gitbook/assets/image%20%281%29.png)

4. Enter the following Code in the Cloud Shell\(use the copy helper at the right\)

```
ibmcloud target -r eu-de -g lab-users
```

![This is the Account and Resource Group you should be connected](.gitbook/assets/image%20%283%29.png)

