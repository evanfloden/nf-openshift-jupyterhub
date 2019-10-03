# nf-openshift-jupyterhub
Configuration for launching Nextflow in OpenShift/k8s with JupyterHub


## Steps to create environment

1. Login to OpenShift with admin rights

2. Create a new project (if required):
    `oc new-project nf-in-jupyter``

3. Create the app:
    ```
    oc new-app learning-portal-template.yaml --param PROJECT_NAME=`oc project --short`
    ```
    *NB: cluster subdomain*

4. Launch the app via the new address

This creates a new environment for each user.