# Jenkins Slave for Node 6 and NPM 3

## Usage

Uses the [RHEL Jenkins Slave Base Image](https://access.redhat.com/containers/#/repo/581d2f3f00e5d05639b6515b), so the build needs to be performed on a registered RHEL host (e.g. OpenShift)

Be sure to label the resulting imagestream with `role=jenkins-slave` per [the docs](https://docs.openshift.com/container-platform/3.4/using_images/other_images/jenkins.html#using-the-jenkins-kubernetes-plug-in-to-run-jobs)