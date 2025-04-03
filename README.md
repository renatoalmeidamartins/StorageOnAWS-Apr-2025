# StorageOnAWS-Apr-2025

## Trainer info:
- email: renatoalmeidamartins@gmail.com
- Linkedin: https://www.linkedin.com/in/renatodealmeidamartins/

## Course materials
- Skill builder: https://skillbuilder.aws/
- Launching the meeting through here: https://classrooms.aws.training
- Lab and course materials here: https://us-east-1.student.classrooms.aws.training/class/ilt%23g4L4N46wPrf3iVkTDxuVE8
- Course update info and list of all available courses: https://releases.awstc.com/
- 
## Day 1 links
- [Well-architected framework](https://aws.amazon.com/architecture/well-architected/?wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc&wa-guidance-whitepapers.sort-by=item.additionalFields.sortDate&wa-guidance-whitepapers.sort-order=desc)
- [AWS Global infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/?p=ngi&loc=1)
- [IAM Policy Simulator](https://policysim.aws.amazon.com/)
- [Beyond 11 9s of durability: Data protection with S3](https://www.youtube.com/watch?v=XyRdMT4zUrA)
- [Dive deep on Amazon S3](https://www.youtube.com/watch?v=sYDJYqvNeXU)
- [Old S3 path-based URLs](https://aws.amazon.com/blogs/aws/amazon-s3-path-deprecation-plan-the-rest-of-the-story/)
- [S3 server access log format](https://docs.aws.amazon.com/AmazonS3/latest/userguide/LogFormat.html#log-record-fields)
- [Policy Generator](https://awspolicygen.s3.amazonaws.com/policygen.html)
- [IAM Policy Reference](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies.html)
- [KMS bucket keys, a cost saving measure](https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucket-key.html)
- [Pre-signed URLs for S3](https://docs.aws.amazon.com/cli/latest/reference/s3/presign.html)
- [S3 access points, ACLs and bucket policies](https://aws.amazon.com/blogs/security/iam-policies-and-bucket-policies-and-acls-oh-my-controlling-access-to-s3-resources/)
- [AWS Comprehend Lambda examples](https://github.com/aws-samples/amazon-comprehend-s3-object-lambda-functions/tree/main)
- [Dealing with multipart uploads](https://docs.aws.amazon.com/AmazonS3/latest/userguide/mpuoverview.html)
- [Using the TransferUtility .Net helper class to automatically manage multipart uploads](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HLuploadDirDotNet.html)
- [Using the TransferManager Java helper class to help with multipart uploads](https://sdk.amazonaws.com/java/api/latest/software/amazon/awssdk/transfer/s3/S3TransferManager.html)
- [Transfer accelaration test](https://s3-accelerate-speedtest.s3-accelerate.amazonaws.com/en/accelerate-speed-comparsion.html)
- [S3 MFA delete](https://docs.aws.amazon.com/AmazonS3/latest/userguide/MultiFactorAuthenticationDelete.html?icmpid=docs_amazons3_console)
- [Object lock](https://docs.aws.amazon.com/AmazonS3/latest/userguide/object-lock.html) - be careful!!!. If locked in compliance mode, the only way to shorten the duration is closing the AWS account. Maximum lock duration is 1000 years.
- [Multi-region access points](docs.aws.amazon.com/AmazonS3/latest/userguide/MultiRegionAccessPoints.html)

## Day 2 links
- [RAID](https://en.wikipedia.org/wiki/RAID)
- [Multi-attach EBS volumens](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-volumes-multi.html)
- EBS storage activitity requirements (volume types for each case):
  - New application requirements are as follows:
    - Requires four block storage volumes:
      - 1 x 10 GiB boot volume
      - 1 x 150 GiB application volume
      - 1 x 60 GiB transaction log volume
      - 1 x 5 TiB data retention volume
    - Minimum of 3000 IOPS, maximum of 9000 IOPS for all four volumes.
    - Throughput requirement of 100 MiB/s or less for all four volumes.
    - Requires point-in-time consistency for recovery time objectives and recovery point objective capabilities.![image](https://github.com/user-attachments/assets/636749ab-610a-440b-9924-fbd28bd693a3)
  - [Fast Snapshot restore](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-fast-snapshot-restore.html)
  - [Cross-account shareing of snapshots](https://docs.aws.amazon.com/ebs/latest/userguide/ebs-modifying-snapshot-permissions.html) - different from what the slide on Module 5 says, when we share a snapshot with another account, it will be in the same region.
  - [EFS performance specifications](https://docs.aws.amazon.com/efs/latest/ug/performance.html)
## Day 3 links
- Topics not covered on S3
  - [CORS (Cross-origin resource sharing)](https://docs.aws.amazon.com/AmazonS3/latest/userguide/cors.html)
  - [Static website hosting](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html?icmpid=docs_amazons3_console) - Amplify Hosting is now favored
  - [FSs storage gateway no longer available, must be migrated to FSx for Windows](https://aws.amazon.com/blogs/storage/switch-your-file-share-access-from-amazon-fsx-file-gateway-to-amazon-fsx-for-windows-file-server/)
  - [CLoud provider support for DataSync](https://docs.aws.amazon.com/datasync/latest/userguide/transferring-other-cloud-storage.html)
