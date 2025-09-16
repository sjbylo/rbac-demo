# Simple RBAC demo for OpenShift Virtualization

1. Apply the `htpasswd.txt` (all passwords are `password`) content to the cluster by creating an htpasswd auth configuration via the Console.
  1. CLuster Settings -> Configuration -> OAuth -> Add HtPasswd and paste the content of the htpasswd file.
1. Create a `demo` project and add a test VM.
1. Apply the cluster role and add (bind) to the user: oc apply -f yaml

After authenticating as user0/password via the Console, cannot create and delete a VM.

