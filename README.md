# s3-secure-backup-recovery
# Secure Backup & Recovery Using Amazon S3

## Project Overview
This project demonstrates how to store files securely in Amazon S3, preserve previous versions, and recover earlier file content.

## AWS Services
- Amazon S3
- S3 Bucket Versioning

## Bucket Configuration
- Bucket name: s3-bucket123344
- AWS Region: eu-north-1 (Europe - Stockholm)
- Bucket Versioning: Enabled
- Public Access: Blocked
- Default Encryption: SSE-S3

## Implementation
1. Created an Amazon S3 bucket.
2. Enabled Bucket Versioning.
3. Uploaded a file named backup-test.txt.
4. Modified the local file and uploaded it again using the same name.
5. Examined the file versions stored in S3.
6. Retrieved the older version to verify that earlier content could be recovered.

## Test Results
The experiment demonstrated that uploading a file with the same name creates a new current version when Versioning is enabled, while previous versions remain available unless deleted.

## Security
- Block Public Access is enabled.
- Server-side encryption uses SSE-S3.
- Bucket access should be granted only to authorized users and services.

## Cost Considerations
Stored object versions consume storage and may incur charges. Storage usage should be monitored to manage costs.

## Skills Demonstrated
- Amazon S3
- Cloud storage
- Object versioning
- Backup and recovery
- Basic cloud security
