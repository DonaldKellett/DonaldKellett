### Hi there 👋

I am currently a Cloud Technical Specialist at Enfinity Solutions Limited, with my current role focused on:

- Architecting and delivering cloud-native solutions to our customers on **AWS** and **Alibaba Cloud**, and
- Daily operations and maintenance of our on-premises **GitLab** and **Kubernetes** infrastructure

In my spare time, I write blog posts on DevOps practices and tools on my personal website: [donaldsebleung.com](https://www.donaldsebleung.com/)

_Subscribe: [![RSS](https://www.donaldsebleung.com/assets/images/rss-logo-32x32.png)](https://www.donaldsebleung.com/feed/rss) [![Atom](https://www.donaldsebleung.com/assets/images/atom-logo-32x32.png)](https://www.donaldsebleung.com/feed/atom) [![\[Valid RSS\]](https://www.donaldsebleung.com/assets/images/valid-rss-rogers.png)](https://validator.w3.org/feed/check.cgi?url=https%3A%2F%2Fwww.donaldsebleung.com%2Ffeed%2Frss) [![\[Valid Atom 1.0\]](https://www.donaldsebleung.com/assets/images/valid-atom.png)](https://validator.w3.org/feed/check.cgi?url=https%3A%2F%2Fwww.donaldsebleung.com%2Ffeed%2Fatom)_

## Work Experience

### Cloud Technical Specialist at Enfinity Solutions Limited (2023/07-present)

#### Terraform migration to OpenTofu (2024/05; 1 month)

Performed a successful migration of all existing internal and customer-owned Terraform IaC projects to OpenTofu following the officially supported procedure outlined in the OpenTofu documentation, for a total of 8 projects

##### Business impact

Eliminated the potential legal risks of managing internal and customer-owned infrastructure with proprietary tooling, ensuring the sustainability of affected IaC projects in the long run

#### Rancher RKE2 OIDC integration with Dex (2024/02; 1 month)

Implemented a centralized identity management solution backed by Active Directory for on-premises Rancher RKE2 cluster, leveraging Dex as the OIDC connector

##### Business impact

Consolidated authN + authZ under a single umbrella across on-premises IT infrastructure with Active Directory as the sole IdP and single source of truth, ensuring the scalability of access management for on-premises resources in the long term

#### Kasten K10 DR drill (2024/01; 1 month)

Performed a successful on-premises DR drill for GitLab EE 16.x and supporting Rancher RKE2 infrastructure with Kasten K10 for cross-cluster application level backup and disaster recovery, with:

- Ansible for automated provisioning of new Rancher RKE2 cluster in a 3-server HA control plane setup with CIS-1.23 hardening
- A confirmed RPO of 48 hours based on daily Kasten K10 backup
- A confirmed RTO of 24 hours based on the actual DR drill duration for complete service resumption of GitLab EE 16.x (and other supporting services)

##### Business impact

Confirmed that the DR handbook procedure is fully functional and actionable, ensuring business continuity in the event of a complete infrastructure failure

#### Kasten K10 DR planning and evaluation (2023/12; 1 month)

Drafted a comprehensive DR handbook for on-premises GitLab EE 16.x installation and supporting Rancher RKE2 infrastructure leveraging Kasten K10 for cross-cluster application-level backup and recovery, followed up by an initial DR test drill on AWS leveraging an automation stack for efficiency, reproducibility and standardization, developed in-house with:

- OpenTofu for provisioning AWS resources mirroring the on-premises infrastructure
- Ansible for provisioning a fresh Rancher RKE2 cluster in a 3-server HA control plane setup with CIS-1.23 hardening on provisioned infrastructure
- GitLab CI with manual approval step for E2E validation of the complete OpenTofu + Ansible automation stack

##### Business impact

Confirmed the feasibility of performing the procedures outlined in the DR handbook and uncovered fundamental limitations of a lift-and-shift recovery of on-premises Rancher RKE2 infrastructure to AWS, laying the groundwork for performing a complete DR drill going forward and ensuring business continuity in the event of a complete infrastructure failure

#### GitLab EE 16.x installation and tuning (2023/07-2023/09; 3 months)

Deployed GitLab EE 16.x to on-premises Rancher RKE2 cluster to accelerate software delivery and enable DevOps, DevSecOps and GitOps workflows, with:

- Rancher RKE2 deployed in HA mode (3 server nodes) for fault tolerance
- Rancher RKE2 deployed with CIS-1.23 profile enabled for security hardening
- Prometheus and Grafana for monitoring, observability and email alerting
- Flux v2 for cluster-wide GitOps management with Microsoft Teams notifications and alerting

##### Business impact

Enabled rapid prototyping, drastically reduced time to production and standardized software delivery processes with a security-first approach

#### Multi-cloud monitoring, observability and alerting (2023/08; 1 month)

Implemented dashboards exporting instance and host-level metrics from 30+ cloud VMs across AWS and Azure for a major airline company, with:

- Amazon CloudWatch for monitoring and observability
- Amazon SNS for email alerting on storage-related events
- AWS Lambda with a container-based deployment model for recurring critical alarms
- GitLab CI for an automated DevSecOps workflow involving multiple pipelines:
    - Terraform pipeline with GitLab-managed remote backend and manual apply step for semi-automated provisioning and management of AWS infrastructure (CloudWatch, SNS)
    - Container-oriented pipeline with unit tests, SAST, image build, Trivy scan and push to Amazon ECR for automated deployment and quality assurance of Lambda-based microservices

##### Business impact

Real-time visibility into AWS and Azure infrastructure, improving SLA and reducing incident response times

### Specialist in IT consulting at China Resources Enterprise Limited (2021/07-2023/05; 1 year 10 months)

Assisted in meeting room setup for videoconferencing, Windows desktop and laptop software installation, Windows and Outlook troubleshooting, printer troubleshooting at Wan Chai HQ office

#### FortiGate to H3C HQ firewall replacement (2023/01-2023/03; 3 months)

Oversaw the technical execution of the HQ firewall replacement from FortiGate to H3C for a BU in the catering industry, jointly devised and executed an appropriate action plan with a Chinese network service provider during off-hours to minimize business disruption and ensure business continuity

##### Business impact

Improved the network security of the affected BU by retiring an EOL firewall product and contributed to the enforcement of Chinese SOE compliance requirements

#### Leased line replacement (2022/10; 1 month)

Oversaw the replacement of a leased line affecting the HQ network topology for a BU in the catering industry, devised and executed an appropriate action plan modifying the HQ FortiGate firewall configuration during off-hours to minimize business disruption and ensure business continuity

##### Business impact

Optimized the network topology for the affected BU, reducing network latency and error rates

### Software Developer (Intern) at M-Labs Limited (2020/06-2020/11; 6 months)

#### Implementing sorting network for ARTIQ control system (2020/09-2020/11; 3 months)

Implemented the sorting network for the ARTIQ control system used in physics experiments, leveraging:

- nMigen for its Python DSL
- Yosys / SymbiYosys for formal verification

#### Porting Minerva RISC-V soft core from Verilog to nMigen (2020/06-2020/08; 3 months)

Ported the Minerva RISC-V (RV32M) soft core from Verilog to nMigen, leveraging:

- Python for its powerful abstractions and language features
- Automated SMT solvers (Yosys, SymbiYosys) for verifying the functional correctness of the FPGA core

### Teaching Assistant (Intern) at BSD Education (formerly BSD Academy) (2016/08; 2 weeks)

Assisted in teaching duties for 2 classes of students aged 8-10 on frontend development with HTML5+CSS3+JS

## Education

BEng. Computer Science and Engineering (4Y), The Hong Kong University of Science and Technology, Class of 2021, First Class Honors, GGA: 3.742

## Community

- Blogging on DevOps practices and tools on [donaldsebleung.com](https://www.donaldsebleung.com/)
- PR contributor to [CNCF Sandbox](https://www.cncf.io/sandbox-projects/) and [Linux Foundation](https://www.linuxfoundation.org/) projects
- Former community moderator on [deepin Forums](https://bbs.deepin.org/user/287133) \(2023 Q2-Q3\)
- PR contributor to [deepin GNU/Linux](https://github.com/linuxdeepin) projects

## Contact

Please kindly refer to my profile and CV for details.
