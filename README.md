# OpenShift V3 Cron Job Example traditional

This Example shows a possibility to easily use traditional cron jobs as Pod on OpenShift V3

The cronjobs defined in etc/crontab will be executed in the given Pod

## How To use

```
$ oc new-app https://github.com/appuio/example-cron-traditional.git --strategy=docker
```

# Bestpractice Cron Jobs on OpenShift

Cronjobs should be triggered from the platform itself as run once Containers. At the moment this functionality is not yet included, but will come with Kuberenetes Version V1.3 (https://github.com/kubernetes/kubernetes/pull/11980)
