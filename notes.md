#### 0420
1. IAM: Separation of access
    - IAM doesn't require region selection
    - Account alias 
    - MFA (root access keys are not recommended)
    - 
    - 
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
   - Types: 
     - Identity based: can attach to a principle (IAM user/role/group)
       - Managed policies: AWS or customer managed
       - Inline policies
     - Resource based: can attach to a resource, such as S3 bucket.
       - Are only inline policies
4. 
