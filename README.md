# AWS-CF-AdJoin
Automate the join to the Active Directory

* **Administrators**: the list of AD groups that should be added as local admins
* **Tag name & tag values**: The name and values of the tag that the EC2 needs to have to be join to the Active Directory

You can optionaly send logs to a dedicated s3 bucket

This only works for Windows instances, linux instances shall be managed through SSM session manager. The instance needs to be SSM ready ([agent installed](https://docs.aws.amazon.com/systems-manager/latest/userguide/sysman-install-ssm-win.html) & proper [instance profile](https://docs.aws.amazon.com/systems-manager/latest/userguide/setup-instance-profile.html))
