**Reflection on Setting Up My AWS Environment**
**Introduction**
Setting up an AWS environment securely is the first step in protecting the integrity and security of cloud resources. This reflection captures the process of setting up my AWS environment as I implemented best security practices. The key topics covered are creating a non-root IAM user, enabling Multi-Factor Authentication (MFA), managing permissions, and implementing access control policies.

**Security Measures Implemented**
1. Non-Root User Setup
  To minimize security risks, I did not employ the AWS root account for regular operations. Instead, I:

Created a standalone IAM user with admin privileges.
  Left the root user disabled for regular activities.
  Assigned permissions in best practices and avoided granting unnecessary access.

2. Activating Multi-Factor Authentication (MFA)
  To protect logins and prevent unauthorized access:
  I enabled MFA for the root account to introduce an extra verification step.  
  I also switched on MFA for IAM users, reducing further the risk of unauthorized access.

4. IAM Permissions and Role-Based Access Control
  I delegated Administrator Access to my IAM user for AWS resource administration.
  Future development includes defining custom IAM roles for different jobs in an effort to reduce over-permissioning.

6. Secure Access Key Management
  Stopping unauthorized access resulting from compromised credentials:
  I created access keys for IAM users but rotated them at regular intervals and stored them safely.

**Conclusion**
Configuring my AWS environment with security in mind has reinforced the importance of least privilege, MFA, and access control concepts. Not utilizing root accounts and using appropriate IAM policies has established a solid foundation for securely controlling AWS resources. I will continue further to hone access policies and examine AWS Security Hub and CloudTrail to further enhance monitoring and compliance.
