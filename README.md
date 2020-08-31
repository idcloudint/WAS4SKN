# WebSphere Application Server 9 FAQ

## 1. When to use WAS Network Deployment (ND) or WAS BASE?  
WAS ND is needed when customer runs 2 or more active nodes of WAS. Customer running only 1 node of WAS needs only WAS Base.
  
## 2. Supported OS:  
https://www.ibm.com/software/reports/compatibility/clarity-reports/report/html/softwareReqsForProduct?deliverableId=021B4E70831411EA8A3A455AB35F5E2C&osPlatforms=AIX|HP|IBM%20i|Linux|Solaris|Windows&duComponentIds=S001|C003|C002&mandatoryCapIds=13|132&optionalCapIds=341|9|39|8|132|20|223|26|40  
  
## 3. Supported DB:  
Any database with a JDBC driver that is compliant with JDBC specification version 4.1 or earlier  
  
## 4. Installation of Trial of WAS:  
  
1. Download and install IBM Installation Manager  
Link to download IBM Installation Manager: https://www.ibm.com/support/fixcentral/swg/selectFixes?parent=ibm~Rational&product=ibm/Rational/IBM+Installation+Manager&function=all  
  
2. Add the following Repository in Installation Manager and install WebSphere  
http://www.ibm.com/software/repositorymanager/com.ibm.websphere.BASE.v90  
  
Full Guide: https://www.ibm.com/support/knowledgecenter/en/SSEQTP_9.0.5/com.ibm.websphere.installation.base.doc/ae/tins_productfiles_im.html  

## 5. Do you charge for development and test server?  
Yes  
  
## 6. Do you charge for active DR?  
Yes  
  
## 7. Do you charge for passive DR?  
No  
  
## 8. What are the terms of using warm backup?  
1.       On the secondary site, IBM WAS can be up but there must be no access of the production data (ie. Cannot use the secondary site to do report generation, UAT, etc).  
2.       On the secondary site, backup of the IBM WAS or IBM WAS configuration server is permitted.  
3.       On the secondary site, patching and update can be done but can only be tested using the 4x72 hours of DR testing, that mean, we can only test all the update quarterly.  
4.       For BUs that wants to switch over to the DR setup and run from the DR setup for a period of time, the primary site have to be switch to passive for that period.   
5.       On the secondary site, a backup system must be available to perform backup operation in the events BUs decided to run on the DR setup for a period of time.  
  
## 9. Link to IBM PVU Table  
https://www.ibm.com/software/passportadvantage/pvu_licensing_for_customers.html  
  
