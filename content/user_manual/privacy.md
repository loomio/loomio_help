---
title: Privacy and Security Information
menu:
  main:
    name: Privacy & Security
    parent: user_manual
---

<!-- - fully gdpr compliant.
- no external trackers
- export all your data, anytime.
- data belongs to the group and is shared history. we do no delete your comment and vote data when you go. that is only available to your group admins.
- our employee security policies
- hosting in EU available. -->

## Privacy

### Group privacy
As a group coordinator, you can customise your privacy and access permissions to suit what your group needs. See the [Loomio User Manual](https://help.loomio.org/en/user_manual/groups/settings/) for more information about Group Settings.

### Privacy Policy
Loomio’s [Privacy policy](https://www.loomio.org/privacy) outlines how we handle personal data. We respect personal privacy and will never sell your data to third parties, nor put advertising into Loomio. We only transfer personal information to third parties where absolutely necessary.

### GDPR Compliance
Loomio complies with European Union General Data Protection Regulations (GDPR). Our [compliance statement](https://www.loomio.org/gdpr) outlines how you can exercise your rights under the GDPR.

## Security
The Loomio software is available for inspection and regularly subject to third party security scan. Please contact us if you’d like to run a PEN test or security scan.

## Software Information

### Loomio’s software license
Loomio software is licensed under [GNU Affero General Public License v3.0](https://github.com/loomio/loomio/blob/master/LICENSE.txt)

### Terms of Service
Loomio’s software service is subject to our standard [Terms of Service](https://www.loomio.org/terms_of_service).

If you represent a New Zealand Government agency, the [Terms of Service for the New Zealand Government](https://drive.google.com/open?id=1VnVE8dlYp_Vr8uuz_8uErWdooZXR469U) apply. The terms are the same as our standard, but with the indemnity clause removed.

### Software maintenance and change management
Loomio software is constantly evolving. Software updates include release notes notifying of new features and changes in the software.

## Hosting Information

### Loomio.org

#### Hosted service provider
Heroku is a cloud application platform used by organizations of all sizes to deploy and operate applications throughout the world. Heroku’s platform provides infrastructure management, scaling, and security.

Heroku applies security best practices and manages platform security, protecting customers from threats. Heroku applies security controls at every layer from physical to application, isolating applications and data, and rapidly deploys security updates without customer interaction or service interruption.

More information can be found at [Heroku’s security policy](https://www.heroku.com/policy/security).

Heroku utilises ISO 27001 and FISMA certified data centres managed by Amazon. Information about security at Amazon data centres is available [here](https://aws.amazon.com/security/).

#### Backup data and Recovery
Loomio software and data recovery are managed by Heroku. The software and data is automatically backed up as part of the deployment process on secure, access controlled, and redundant storage.  Heroku use these backups to deploy the Loomio software and data across the platform and automatically bring the application back online in the event of an outage.

More information can be found at [Heroku’s security policy](https://www.heroku.com/policy/security).

#### govt.loomio.nz

govt.loomio.nz is an instance of Loomio running on Amazon Web Services (AWS) datacenters in Sydney, Australia, which is approved for NZ Government data processing.

New Zealand Cloud Security and Compliance information is available [here](https://aws.amazon.com/compliance/new-zealand-data-protection/).

## Third Party Security Assessment

Loomio software and service has been assessed by:

- eHealth Systems, SA Health, Government of South Australia - Security Scan (by IBM Security AppScan Standard 9.0.3, December 2018)
- New Zealand Government Marketplace: Loomio currently holds Tier 3 security status.  For more information, see [Marketplace.govt.nz - Cloud services security risk and assurance](https://marketplace.govt.nz/suppliers/apply-to-be-a-supplier-2/cloud-services-security-risk-and-assurance/)
- New Zealand Government Ministry of Social Development - Cloud Computing User Assessment
- NZTA Security Scan by Aura Information Security.

## Frequently Asked Questions about Privacy and Security

### Change Control
_Q: The Loomio service is a shared platform and an open source application - does the organization maintain a change control Policy with the maintenance of an audit trail of changes to the production environment?_

A: Loomio software is open source, owned and maintained by Loomio Cooperative Limited.

We review and test all contributions to the software ourselves before anything is accepted into the final build. In practice more than 99% of the software has been developed by Loomio Cooperative. Open source commits tend to be minor and few.

All changes to the software are recorded in our Git repository, which provides a cryptographic secure history of all changes since the project began.

Loomio software has a extensive automated testing suite which is run before any new version of the software is deployed.
Our database is managed by Heroku and provides continuous protection, meaning we can rollback to any point in time.

All changes to our production system are logged within Heroku.

### Loomio’s password policy
_Q: What are the requirements for a Loomio registration password? E.g minimum length and complexity._

A: The minimum length required for Loomio’s platform is 8 characters. We require that passwords are not on the list of the [10,000 most commonly used passwords](https://en.wikipedia.org/wiki/Wikipedia:10,000_most_common_passwords).

We don't use passwords by default; users generally login via link sent to their email address. Users who specifically request to use passwords will have them enabled on their accounts.

This means that our user accounts are no weaker than the user's email provider.

Please see the [Loomio User Manual](https://help.loomio.org/en/user_manual/users/sign_in/) for more information about user sign-in.

### Inactive sessions

_Q: What is the timeout period for inactive sessions?_

A: We don't have a session timeout. If an organization has a timeout requirement, we recommend this is implemented at the computer session level rather than application session.

### Notifiable incidents

_Q: How are customers informed of security breaches (should they occur)?_

A: By email. We notify customers as soon as we can, and no later than 72 hours from when we become aware of a security breach.

### Personnel screening

_Q: Do privileged users (administrators of the system) undergo any form of security clearance prior to being granted access?_

A: Loomio staff and cooperative members may, in the course of their work, have access to customer data including personal data as described in Loomio’s [Privacy Policy](https://www.loomio.org/privacy).

Employee and contractor agreements for people working at Loomio include confidentiality clauses to protect Loomio and customer confidential information.  We treat all customer information and data as confidential, except for situations where a customer has explicitly made the information publicly accessible.

Access to the database, where discussion and decision data is held, is tightly controlled and protected internally within Loomio under the following restrictions:

- Loomio’s internal security principle is that customer data is only accessed after permission has been granted by the customer, or the customer has requested help with an issue.
- When it is necessary to maintain the system.
- Loomio workers with access to the customer database must be highly experienced software developers, compliant with Loomio's privacy policy, and in most cases they will be a co-owner member of Loomio Cooperative with associated responsibilities.
- Access to the Loomio database is available to no more than five Loomio staff members,  controlled by Loomio Cooperative members who have been working in the development and maintenance of Loomio for more than four years.

As a registered worker cooperative, Loomio is collectively owned by its members, who are all equal shareholders in the Cooperative and hold the responsibilities of business co-owners. Details and responsibilities of membership are outlined in the [Loomio handbook](https://loomio.coop/).

You can read more about Loomio’s policy for data security, integrity and access in our [privacy policy](https://www.loomio.org/privacy). We specifically draw your attention to the following:

_Loomio will not sell or rent any information you share with us. Access to your content and personally identifiable information is tightly controlled internally. Loomio takes all reasonable steps to protect your content from loss, misuse and unauthorized access, disclosure, alteration and destruction._

### Data Encryption

_Q: Is Loomio data encrypted?_

A. We use TLS (Transport Layer Security) encryption for data sent between Loomio and users where they are using a securely hosted email service.

You can read more about Loomio’s policy for data security, integrity and access in our [privacy policy](https://www.loomio.org/privacy). We specifically draw your attention to the following:

_Content entered into the platform is distributed to the appropriate members of your groups via secure connections where possible and sent via email in the normal course of operation. Your content is only as secure as the personal devices, email services, ISPs, and actions of the members of your group._

### Accessibility
Loomio complies with the New Zealand Web Accessibility Standard, which requires support of the Web Content Accessibility Guideline (WCAG) 2.0 conformance levels A and AA. Loomio also conforms with much of Level AAA.  

Loomio is committed to accessibility. We work with recognized Canada-based web accessibility consultant [David Best](http://www.davebest.info/), and we regularly test core functions of the software for accessibility.  

“Loomio has done a great job with integrating the WCAG standards. However, screen reader user feedback is critical in measuring the usability of Loomio. The web pages are designed with a common look and feel layout of Regions and Heading hierarchy for ease of keyboard navigation. I believe Loomio should be compatible with most screen readers, and it was primarily tested with the JAWS screen reader. Please encourage your screen reader users to help improve Loomio with their feedback.” **David Best**
