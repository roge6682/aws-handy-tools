# aws-automation-tools
**Handy AWS automation tools** <br>
This repo consists of a variety of handy aws automation tools. This README attempts to provide some guidance on how to use each tool,<br>
**TOOL:** EC2 Instance Tag Automation <br>
**Script:** tag_instances3.py <br>
**Use case:** Used to modify instances tag to align with your organization tagging policy. <br>
  **How to use tagging automation script** <br>
   - what you'll need:
     1. Python<br>
     2. boto3 library<br>
     2. awscli<br>
     3. aws account with creds<br>
     4. clone repo and run python script<br>
        ```
        $ git clone https://github.com/roge6682/aws-handy-tools.git
         Cloning into 'aws-handy-tools'...
         remote: Enumerating objects: 9, done.
         remote: Counting objects: 100% (9/9), done.
         remote: Compressing objects: 100% (7/7), done.
         remote: Total 9 (delta 0), reused 6 (delta 0), pack-reused 0
         Receiving objects: 100% (9/9), done.
         $ ls
         aws-handy-tools/
         $ cd aws-handy-tools/
         $ ls
         README.md  get_iam_users.py  host_ids  tag_instances3.py
         ```
     5. ec2 instance(s) to test with. Launch instance(s) in your aws with very minimal resources, then get instances ids and save in a file like so:
        ```
        aws ec2 describe-instances --query 'Reservations[*].Instances[*].InstanceId' --output text > instance_ids
        ```



