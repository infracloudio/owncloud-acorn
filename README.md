# ownCloud
 About  Acornfile for running ownCloud on Acorn.

 ## Deploy the ownCloud App 

You can deploy the sample web app on the Acorn SaaS Platform to test the Application.

## ownCloud Acornfile

Let us have a close look at the Acornfile and see what is defined:

- **Containers**: These are the containers that will be deployed for running ownCloud. We have two containers, one for ownCloud and the other for Redis. We are setting the environment variables returned from the MariaDB Acorn service for the ownCloud container.
- **Services**: Services in Acron are external services that your application can utilize. In this case, we are using the [MariaDB Acorn service](https://github.com/acorn-io/mariadb/pkgs/container/mariadb).


## Steps

1. Login into the Acorn SaaS Platform using the Github Sign-In option with your Github user.
2. You can select the "Create Acorn" option to create new Acorns and deploy your Application.
3. Choose the source for deploying your Acorns
  * Select "From Acorn Image" to deploy the sample Application and select its Image
  * Provide any random name such as `web-app` and keeping Project's default Region, type in the below Acorn image and choose Create 
    ```bash
    ghcr.io/infracloudio/owncloud-acorn:v0.0.2
    ```
4. Now the sample App is provisioned on the Acorn SaaS Platform and is available for **up to 2 hours**.
5. Once the Acorn is running, you can access it by clicking the Endpoint or the redirect link.

## Acorn Nextcloud App Details

The Acorn Dashboard is integrated with multiple features such as Events, Logs, Details, and access to the Shell of the Application. Details include the CPU, Memory, Network, Latency, Requests, and Errors for the Application.

Explore various available options by clicking the Menu option on your Acorn App.

For more details on using the Acorn Dashboard, check this link - 

## Edit the Acorn Application

You can edit your Acorn's Image and Advanced Options by selecting the Edit option 

## Remove Acorn Application

To Remove the Acorn, select the Remove option from your Acorn's Menu.
