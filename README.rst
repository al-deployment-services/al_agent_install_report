Sample usage of Alert Logic API to check AL Agent install status
================================================================
This is a demonstration script on how to use Alert Logic Cloud Defender and Cloud Insight API in order to check status of AL Agent installation in your environment.

Two API end-point that will be used in this demonstration:

* Cloud Defender API (https://docs.alertlogic.com/developer/)
* Cloud Insight API (https://console.cloudinsight.alertlogic.com/api/#/)


Requirements
------------
* Alert Logic Account ID (CID)
* Credentials to Alert Logic Cloud Insight (user name and password, or access key and secret key)
* Credentials to Alert Logic Cloud Defender API (API KEY)

Restrictions
---------------
* Currently by default the script will filter all Cloud Insight Security Appliance
* There is no filter for Threat Manager appliance due to the nature of naming nomenclature that is decided by customer
* This sample script will check both parent Alert Logic CID and the respective child, your credentials must have access to child CID


Sample Usage
------------
Replace the sample parameter with your information and execute the script ::

    python al_agent_install_report.py -cid 99999 -dc ASHBURN -u first.last@company.com -p MyCloudInsightPassword -a MyCloudDefenderAPIKey

All output will be grouped by CID and AWS account number.


Arguments
----------
  -cid    Alert Logic Customer CID
  -dc     Your data residency (ASHBURN, DENVER and NEWPORT)
  -u      User name or access key for Cloud Insight authentication
  -p      Password or secret key for Cloud Insight API Authentication
  -a      Cloud Defender API Key

Contributing
------------
Since this is just an example, the script will be provided AS IS, with no long-term support.

License and Authors
===================
License:
Distributed under the Apache 2.0 license.

Authors:
Welly Siauw (welly.siauw@alertlogic.com)
