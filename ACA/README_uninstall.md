# IBM® Business Automation Content Analyzer
=========

## Introduction

This readme provide instruction to deploy IBM Business Automation Content Analyzer with IBM® Cloud Pak for Automation platform. IBM Business Automation Content Analyzer offers the power of intelligent capture with the flexibility of an API that enables you to extend the value of your core enterprise content management (ECM) technology stack and helps you rapidly accelerate extraction and classification of data in your documents. 


Uninstall
-----------
1. Backup your ontology.
2. In the CR yaml file:  comment out `ca_configuration` section

3. Apply the CR.  For example:  `oc apply -f [PATH TO CR YAML]`

4. Delete the all the subdirectories under the CA Data PVC.

5. Delete the all the subdirectories under the CA Config PVC.

6. Delete the all the subdirectories under the CA Log PVC.