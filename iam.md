#### IAM
1. IAM: Separation of access
    - IAM doesn't require region selection
    - Account alias 
    - MFA (root access keys are not recommended)
2. IAM Users and Groups 
    - Users:
      - By default a user doesn't have any permission
      - Create User and update password
      - User doesn't have access beyond set policy
      - ARN: https://docs.aws.amazon.com/IAM/latest/UserGuide/reference-arns.html
    - Groups:
      - Can attach policy to a group 
      - Can add users to group
3. IAM Policy
   - Policy contains different permissions determine whether the request is allowed or denied
   - Stored in JSON docs in AWS
   - Default Deny
   - Types: 
     - Identity based: can attach to a principle (IAM user/role/group)
       - Managed policies: AWS or customer managed
       - Inline policies
     - Resource based: can attach to a resource, such as S3 bucket.
       - Are only inline policies
4. IAM Roles
    - Are not users (can be EC2 instances or applications)
    - Allows you to grant access without long-term access keys (!)
    - Delegation (you grant access to someone) vs Federation (identity provider and AWS)
    - Trust policy vs permission policy
    - Principle can be user, group, or role
    - One role per instance only
    - Cannot add role to IAM group, roles cannot make direct access to AWS services
    - Best practices: ![IAM best practices.png](img%2FIAM%20best%20practices.png)
![best practices 2.png](img%2Fbest%20practices%202.png)
