# Hello, I'm Rexmond Anih 

![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonwebservices&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=githubactions&logoColor=white)
![Microsoft 365](https://img.shields.io/badge/Microsoft_365-D83B01?logo=microsoft&logoColor=white)
![Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID-0078D4?logo=microsoft&logoColor=white)

## Cloud & Infrastructure Engineer | Systems Engineer | Infrastructure Automation

I am a **Cloud & Infrastructure Engineer / Systems Engineer** with over **8 years of IT experience**, working across enterprise infrastructure, cloud platforms, identity, endpoint management, networking, systems administration, and technical operations.

My engineering focus is increasingly centered on building **secure, automated, observable, and repeatable infrastructure** using technologies including **Microsoft Azure, AWS, Terraform, GitHub Actions, Linux, Microsoft Entra ID, Microsoft 365, and Infrastructure as Code**.

I enjoy taking infrastructure through the complete engineering lifecycle:

**Design → Build → Secure → Automate → Validate → Monitor → Document → Operate**

Rather than treating infrastructure as a collection of manually configured resources, I focus on building environments that are:

- **Secure**
- **Automated**
- **Observable**
- **Repeatable**
- **Maintainable**
- **Version-controlled**
- **Operationally sustainable**

---

# Featured Engineering Project

## Multi-Cloud DevSecOps Infrastructure Automation Platform

**AWS • Microsoft Azure • Terraform • GitHub Actions • OIDC • Linux • CloudWatch • Azure Monitor • DevSecOps**

A hands-on multi-cloud infrastructure engineering platform designed and implemented across **Amazon Web Services and Microsoft Azure**.

The project demonstrates the complete lifecycle of modern cloud infrastructure — from networking and compute deployment through Infrastructure as Code, CI/CD, federated identity, security hardening, Terraform modularization, observability, validation, and controlled infrastructure teardown.

### Architecture

```mermaid
flowchart TB

    ENG["Cloud / Infrastructure Engineer"]
    GH["GitHub Repository"]
    GHA["GitHub Actions CI/CD"]
    TF["Terraform"]

    ENG --> GH
    GH --> GHA
    GHA --> TF

    TF --> AWS
    TF --> AZURE

    subgraph AWS["Amazon Web Services"]

        VPC["VPC"]
        PUB["Public Subnet"]
        APP["Private Application Subnet"]
        MGMT["Management Subnet"]

        EC2["Linux EC2"]
        SSM["AWS Systems Manager"]
        VPCE["VPC Endpoints"]

        CW["CloudWatch"]
        SNS["SNS Alerts"]
        KMS["KMS Encryption"]

        VPC --> PUB
        VPC --> APP
        VPC --> MGMT

        PUB --> EC2
        EC2 --> SSM
        EC2 --> VPCE
        EC2 --> CW
        CW --> SNS
        SNS --> KMS
    end

    subgraph AZURE["Microsoft Azure"]

        VNET["Azure VNet"]
        WEB["Web Subnet"]
        AAPP["Application Subnet"]
        AMGMT["Management Subnet"]

        NSG["Network Security Groups"]
        VM["Ubuntu Linux VM"]

        AMA["Azure Monitor Agent"]
        DCR["Data Collection Rule"]
        LAW["Log Analytics Workspace"]

        VNET --> WEB
        VNET --> AAPP
        VNET --> AMGMT

        WEB --> NSG
        NSG --> VM

        VM --> AMA
        AMA --> DCR
        DCR --> LAW
    end
