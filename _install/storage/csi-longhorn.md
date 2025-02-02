# Installation Requirements 
[Ansible longhorn](https://github.com/anarchist117/Ansible/blob/main/longhorn.yml)

# Check Script
```
curl -sSfL https://raw.githubusercontent.com/longhorn/longhorn/v1.8.0/scripts/environment_check.sh | bash
```
```
[INFO]  Required dependencies 'kubectl jq mktemp sort printf' are installed.
[INFO]  All nodes have unique hostnames.
[INFO]  Waiting for longhorn-environment-check pods to become ready (0/0)...
[INFO]  All longhorn-environment-check pods are ready (2/2).
[INFO]  MountPropagation is enabled
[INFO]  Checking kernel release...
[INFO]  Checking iscsid...
[INFO]  Checking multipathd...
[INFO]  Checking packages...
[INFO]  Checking nfs client...
[INFO]  Cleaning up longhorn-environment-check pods...
[INFO]  Cleanup completed.
```

# Documentation
[Install Longhorn on Kubernetes](https://longhorn.io/docs/1.8.0/deploy/install/)
[Using the Environment Check Script](https://longhorn.io/docs/1.8.0/deploy/install/#using-the-environment-check-script)
