# Lab 01 — Deploying an ECS on Huawei Cloud

## 1. Overview

This lab demonstrates how to create and configure an Elastic Cloud Server (ECS) on Huawei Cloud.

**Objectives:**
- Understand the purpose of Elastic Cloud Server (ECS).
- Deploy an Ubuntu Linux virtual machine.
- Configure basic instance settings and network connectivity.
- Verify that the ECS is running and accessible through SSH.

## 2. Architecture

![ECS Architecture](images/architecture.png)

**Architecture Description:**

A Linux ECS is deployed inside a Huawei Cloud VPC and subnet. The ECS is associated with a Security Group to control network access and an Elastic IP (EIP) for public SSH connectivity.

## 3. Resource Configuration

| Resource | Configuration |
|---|---|
| Cloud Provider | Huawei Cloud |
| Region | AP-Jakarta |
| Service | Elastic Cloud Server (ECS) |
| Operating System | Ubuntu 24.04 LTS |
| Instance Flavor | [vCPU / RAM] |
| System Disk | [Type / Capacity] |
| VPC | [VPC Name] |
| Subnet | [Subnet Name] |
| Security Group | [SG Name] |
| EIP | [Enabled / Disabled] |
| Billing Mode | [Pay-per-use / Yearly-Monthly] |

## 4. Implementation

### Step 1 — Create an ECS Instance

1. Log in to Huawei Cloud Console.
2. Navigate to **Compute → Elastic Cloud Server**.
3. Select **Buy ECS** or the equivalent creation option.
4. Choose the region, instance flavor, and operating system.

**Screenshot:**

![ECS Configuration](images/ecs-configuration.png)

### Step 2 — Configure Network & Security

1. Select the VPC and subnet.
2. Assign the appropriate Security Group.
3. Configure EIP connectivity if public access is needed.
4. Configure the login credentials or SSH key pair.

**Screenshot:**

![ECS Network](images/ecs-network.png)

### Step 3 — Deploy ECS

1. Review the selected configurations.
2. Confirm the deployment.
3. Verify that the instance status is **Running**.

**Screenshot:**

![ECS Running](images/ecs-running.png)

## 5. Testing & Validation

### Test 1 — SSH Connection

Connect to the ECS using an SSH client, according to the selected authentication method.

**Expected Result:** The SSH connection is successful.

**Actual Result:** [Pass / Fail]

### Test 2 — Operating System Verification

Execute the following commands:

- `whoami` — Verify the logged-in user.
- `hostnamectl` — Display the operating system and hostname.
- `ip -4 addr` — Display IPv4 addresses.
- `ip route` — Display the system routing table.

**Expected Result:** The ECS displays the expected OS and network configuration.

**Actual Result:** [Pass / Fail]

**Screenshot:**

![ECS Validation](images/ecs-validation.png)

## 6. Troubleshooting

Document any issues encountered during deployment.

| Issue | Root Cause | Resolution |
|---|---|---|
| [Issue] | [Cause] | [Solution] |

*If no issues occurred, write: No issues encountered during deployment.*

## 7. Conclusion

**Results:**
- [ ] ECS successfully deployed.
- [ ] Instance
