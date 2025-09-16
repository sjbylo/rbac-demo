# Simple RBAC demo for OpenShift Virtualization

1. Apply the `htpasswd.txt` file to your cluster by creating an htpasswd OAuth configuration via the Console:
   1. Cluster Settings -> Configuration -> OAuth -> Add HTPasswd and paste the content of the `htpasswd.txt` file.
1. Create a `demo` project and add a test VM.
1. Apply the cluster role and add (bind) to the user: `oc apply -f yaml`
1. Log into the cluster as `user0` with password `password`, navigate to the VM you created in the `demo` project.
1. Note you cannot Create or Delete the VM.


