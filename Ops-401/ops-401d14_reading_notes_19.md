# [Cloud Detective Controls](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html)

1. What are some of the IoCs that GuardDuty can detect?

    GuardDuty can detect indicators of compromise (IoCs) such as unusual API activity, logins from strange locations, and excessive data transfer.

2. What are some of the data sources which GuardDuty can use?

    It utilizes data sources like VPC Flow Logs, DNS logs, and CloudTrail

3. How does GuardDuty use access behavior to spot potential malicious activity?

    By examining access behavior patterns and comparing them with baseline activities, GuardDuty identifies potentially malicious activity, flagging actions like unusual resource access or API calls from unexpected locations