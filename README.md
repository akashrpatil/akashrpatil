Allows remote attackers with portal access to view or raise arbitrary issues in Jira Service Desk projects due to CVE 2019-14994 
https://tickets.metabrainz.org/secure/Signup!default.jspa 


Subdomain: mbz.plex.tv  

https://intel.atlassian.net/servicedesk/customer/user/login  

CVE: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2019-14994

This advisory discloses a critical severity security vulnerability. Versions of
Jira Service Desk Server and Data Center are affected by this vulnerability.

Customers who have upgraded Jira Service Desk Server and Data Center to version
3.9.16, 3.16.8, 4.1.3, 4.2.5, 4.3.4, or 4.4.1 are not affected.

Customers who have downloaded and installed affected versions of Jira Service
Desk Server and Data, please upgrade your Jira Service Desk Server
and Data Center installations immediately to fix this vulnerability.

By design, Jira Service Desk gives customer portal users permissions only to
raise requests and view issues. This allows users to interact with the customer
portal without having direct access to Jira. These restrictions can be bypassed
by a remote attacker with portal access who exploits a path traversal
vulnerability. Exploitation allows an attacker to view all issues
within all Jira
projects contained in the vulnerable instance. This could include Jira Service
Desk projects, Jira Core projects, and Jira Software projects.

Impact
Attacker can raise unlimited issues.
Note that attackers can grant themselves access to Jira Service Desk
portals that have the 'Anyone can email the service desk or raise a request in the portal'
setting enabled. Changing this setting does not defend against an attacker that
has portal access via other means. Atlassian does not recommend changing the setting.
