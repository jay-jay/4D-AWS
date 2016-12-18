# 4D-AWS
AWS (Amazon Web Services) 4D Component

#### Contributors are welcome

## Installation
1. Drop aws.4dbase into your 4D Application's Components folder
2. Under /aws.4dbase/Resources, rename config-sample.json to config.json
3. Enter desired config. 
4. (Optional) If you will use methods that require aws cli then please install AWS CLI. (http://docs.aws.amazon.com/cli/latest/userguide/installing.html)
5. Done

### AWS S3 Sync with CLI
Sync local directory to AWS s3 directory
```
Syntax: aws_s3_cli_sync(local_path ; s3_path)
local_path (Format: /Users/username/Documents/Directory-to-sync/)
s3_path (Format: s3://bucket_name/directory-path-name/
returns TEXT

Example 1:
$response:=aws_s3_cli_sync ($local_path;$s3_path)

```
