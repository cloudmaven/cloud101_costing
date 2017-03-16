---
title: "Calculating and comparing costs"
teaching: 0
exercises: 30
questions:
- "How do I calculate and compare costs for virtual machines and storage between each cloud provider?"
objectives:
- "Learn to create a table of cost comparison"
keypoints:
- Choose comparable virtual machine setups (vCPUs, RAM, SSD,etc.) across the different cloud providers with and calculate and compare teh costs.

---

### We want to create a table that looks like this!

| Resource Type                  | AWS      | Azure  | Google Cloud  | AWS OD Hourly | Azure OD Hourly | Google Cloud OD Hourly |
|--------------------------------|----------|--------|---------------|---------------|-----------------|------------------------|
| Standard 2 vCPU with SSD       | m3.large | D2 v2  | n1-standard-2 | 0.133         | 0.140           | 0.070                  |
| High Memory 2 vCPU with SSD    | r3.large | D11 v2 | n1-highmem-2  | 0.166         | 0.185           | 0.088                  |
| HighCPU 2 vCPU with SSD        | c3.large | F2     | n1-highcpu-2  | 0.105         | 0.124           | 0.053                  |
| Standard 2 vCPU with no SSD    | m4.large | D2 v2  | n1-standard-2 | 0.108         | N/A             | 0.183                  |
| High Memory 2 vCPU with no SSD | r3.large | D11 v2 | n1-highmem-2  | 0.166         | N/A             | 0.201                  |
| HighCPU 2 vCPU with no SSD     | c4.large | F2     | n1-highcpu-2  | 0.100         | N/A             | 0.166                  |

| Storage                        | s3    | Blob Storage | Cloud Storage |
|--------------------------------|-------|--------------|---------------|
| per GB per month (all regions) | 0.023 | 0.02         | 0.02          |

The calculators are located here:

[AWS](https://calculator.s3.amazonaws.com/index.html)

[Azure](https://azure.microsoft.com/en-us/pricing/calculator/)

[Google](https://cloud.google.com/products/calculator/)

**Look closely at RAM and attached storage amount. 
