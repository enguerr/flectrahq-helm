# Package Helm Chart for FlectraHQ
##Flectra
Flectra is a suite of web based open source business apps.
The main Flectra Apps include an Open Source CRM, Website Builder, eCommerce, Warehouse Management, Project Management, Billing & Accounting, Point of Sale, Human Resources, Marketing, Manufacturing, ...

Flectra Apps can be used as stand-alone applications, but they also integrate seamlessly so you get a full-featured Open Source ERP when you install several Apps.
## Status
this helm is not currently production ready but provides a way to execute and test the deployment.

##TODO
- add postgresql waiter in init container to replace this dumb sleep 30... 

## INSTALL
```
helm install -n flectra flectra . -f values.yaml --create-namespace
```
## UPGRADE
```
helm upgrade -n flectra flectra . -f values.yaml
```