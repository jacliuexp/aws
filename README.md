## aws
```
lsblk -o MOUNTPOINT,SERIAL,UUID,NAME
MOUNTPOINT SERIAL               UUID                                 NAME
           vol099475b52699f0057                                      nvme0n1
                                                                     ├─nvme0n1p1
/                               1698b607-b2a7-455f-b2ee-ed7f6e17ed9f └─nvme0n1p2
/mnt       vol0898e1d12557b08f6 1979c86c-e895-4902-a4f8-68f6152a23bd nvme1n1
```

```
curl http://169.254.169.254/latest/meta-data/
ami-id
ami-launch-index
ami-manifest-path
block-device-mapping/
events/
hostname
iam/
identity-credentials/
instance-action
instance-id
instance-life-cycle
instance-type
local-hostname
local-ipv4
mac
metrics/
network/
placement/
profile
public-keys/
reservation-id
security-groups
services/

curl http://169.254.169.254/latest/meta-data/ami-id; echo
ami-04f4cc368426af213
sh-4.2$
```
## S3
```
aws s3 ls s3://dev-chunks --recursive
aws s3 rm s3://dev-chunks --recursive --quiet
```
