
# **Tan Yong Heng**
Singapore

📧 yongheng0905@gmail.com

📞 +65-94301218

[LinkedIn](https://www.linkedin.com/in/tanyongheng)


## **Summary**

Staff platform engineer with 15+ years of experience building internal developer platforms at enterprise scale — still hands-on writing Java pipelines, Kubernetes controllers, and Terraform modules alongside leading squads of 4–12 engineers. At Standard Chartered, owned six platform initiatives that eliminated $2.5M/year in licensing, enabled 300+ teams to shift from monthly to weekly releases, and improved platform availability from 99.5% to 99.95%. Presented the platform modernization strategy to the Technology Council, securing multi-year investment.


## **Areas of Depth**
**Kubernetes platforms:** Designed and operated 8 OpenShift clusters (400+ nodes, 6,000+ pods); built admission controllers, RBAC engines, and namespace provisioning automation.
**Kafka at scale:** Consolidated 14 clusters onto OSS Kafka; capacity planning for 500K msg/sec; MirrorMaker 2 cross-DC replication; schema registry governance.
**Observability & SRE:** Built telemetry pipelines (2 TB/day, 50K events/sec); Prometheus + Grafana + OpenTelemetry; SLO/error budget frameworks; on-call ownership.
**IaC & Cloud:** Authored 12 foundational Terraform modules (200+ consumers); Ansible fleet automation; AWS (EC2, EKS, S3, IAM).
**CI/CD & IDP:** Migrated 2,000+ repos to Azure DevOps; ArgoCD evaluation; platform-as-a-product approach to developer experience.
**Languages:** Java · C# / .NET · Python · HCL · Bash


## **Experience**

### **Platform Engineering Lead**
**Standard Chartered**
*May 2018 – Present*

Technical IC lead across six major platform initiatives — owning architecture, hands-on delivery, and on-call operational ownership. Promoted three times in 6 years (AVP → VP → SVP, equivalent to Senior → Staff → Senior Staff scope). Hired and built three of the six squads from scratch; grew 4 engineers from mid-level to senior and sponsored 2 for tech lead roles. Established architecture decision records (ADRs), blameless postmortem practices, and a platform engineering technical interview bar — all adopted across the wider engineering org (~1,500 engineers).

#### **Key Projects & Impact**

- **Kafka Platform** *(Jan 2026 – Present)*
  - Leading the build-up and consolidation of all existing Kafka infrastructure across SCB bank, migrating workloads onto the current platform.

- **Platform Modernization & Datacenter Migration** *(2022 – 2025)*
  - Led a 12-engineer squad modernizing a legacy integration platform serving 300+ application teams — reducing platform incidents by 65% (from ~20/month to ~7/month) and unblocking the retail banking division's target of weekly releases (up from monthly).
  - Designed geo-resilient, multi-site architecture — chose DNS-based failover over BGP anycast for simplicity and auditability in a regulated environment where change-control overhead for network-layer changes was 3x higher.
  - Personally wrote Helm charts, Ansible playbooks, and rollback automation. Executed the production cutover hands-on; hit a critical LDAP sync failure mid-migration blocking 40 services — diagnosed root cause (stale connection pool config) and patched live within the change window.
  - Rebuilt the observability stack on Prometheus + Grafana (replacing Dynatrace), saving $800K/year in licensing while improving dashboard coverage from 40% to 95% of services.
  - Drove alignment across 8+ enabling platform teams, unblocking 23 cross-team dependencies. Authored the ADR for the dual-runtime architecture (containers + Podman on bare metal) — presented to the Architecture Review Board and adopted as the org-wide reference standard.
  - Deployment pipelines (OpenShift via Helm 3, RHEL9 via Ansible) adopted by 180+ application teams within 6 months.

- **Core Runtime Kubernetes Platform** *(2020 – 2022)*
  - Owned the Internal Developer Platform (IDP) serving 300+ engineers, 8 OpenShift clusters (400+ nodes, 6,000+ pods, 99.9% availability) — chose OpenShift over EKS to meet on-prem compliance requirements while providing a consistent developer experience across environments.
  - Led a 7-engineer team; personally wrote the namespace provisioning controller, RBAC policy engine, and resource quota admission webhooks that automated 80% of previously manual platform requests.
  - Defined standardized deployment workflows (Helm, namespace provisioning, SCC, CRD management) — reducing deployment time from 45 min to 8 min. Authored the ArgoCD/GitOps technical recommendation adopted by the platform org for next-generation rollout.
  - Built platform observability (Prometheus + Grafana) for 8 OpenShift clusters; established SLO dashboards tracking DORA metrics — improved tenant deployment frequency from 2/month to 8/month and reduced change failure rate from 25% to 8%.
  - Improved cluster utilization from 35% to 72% through resource quota tuning and bin-packing optimizations, avoiding $500K in planned capacity expansion.

- **Cloud Enablement** *(2019 – 2020)*
  - Led a 4-engineer squad — first team in the bank to run production workloads on AWS. Personally wrote 12 foundational Terraform modules (VPC, ALB, EC2 ASG, IAM, S3, CloudWatch); modules accumulated 200+ downstream consumers across 50+ teams.
  - Reduced new environment provisioning from 2 weeks (manual ticketing) to 30 minutes (self-service) via Ansible pull, ASGs, and cloud-init patterns.

- **CI/CD Platform Migration** *(2019 – 2020)*
  - Technical lead for migrating 2,000+ repositories from Jenkins to Azure DevOps. Wrote Python tooling to bulk-convert Jenkinsfiles, cutting per-team migration effort from 5 days to 4 hours.
  - Co-developed standardized pipeline templates adopted by 150+ teams, reducing pipeline failures by 30%. Added SAST/SCA scanning stages, catching 400+ dependency vulnerabilities in the first quarter.

- **Observability Platform** *(2018 – 2020)*
  - Built and led a 5-engineer squad that created the Telemetry Hub — SCB's first centralized observability platform. Personally architected and coded the telemetry pipeline (Java + Kafka Streams) processing 2 TB/day and 50K events/sec. Chose Kafka as the transport layer over direct log shipping for backpressure handling and replay capability.
  - Deployed 4 Elasticsearch clusters across 2 regions (regional over cross-DC to keep query latency <200ms and comply with data residency); operated a telemetry agent fleet across 1,200+ instances. Learned the hard way when a FluentBit config push caused a log storm — built canary deployment for agent upgrades afterward.
  - Reduced MTTD from 45 min to <5 min and MTTR by 60% across adopting teams through correlated logs, metrics, and traces. Carried on-call for the platform; ran blameless postmortems that became the template for the wider engineering org.


### **Solutions Architect**
**PALO IT**
*Jun 2017 – May 2018*

- Led a DevOps consulting engagement for a major e-commerce client. Architected an elastic Selenium Grid on AWS (Terraform) — reducing test execution from 6 hours to 15 minutes (24x improvement), unblocking 3 releases/week.
- Established automated infrastructure patterns (Ansible + Packer) adopted as the client's standard across 5 product teams.


### **Software Architect**
**Maloft Pte Ltd** *(returned to lead architecture)*
*May 2016 – Jun 2017*

- Introduced production observability (Elasticsearch, Prometheus) and diagnosed critical latency issues in real-time trading systems (.NET Rx, Redis) — traced root cause to connection pool exhaustion, fixing a bug that had caused intermittent trade failures for months.
- Mentored 3 junior engineers into independent contributors capable of owning production services; established code review and CI pipeline standards.


### **Software Engineer**
**Human Longevity, Inc.**
*Apr 2015 – May 2016*

- Built a landing zone data gateway (C#, HTTP, Kafka) ingesting genomics datasets from 8 partner clinical systems (500+ sequences/day); developed a Jupyter + Spark analysis platform enabling researchers to run variant-calling pipelines on 100TB+ datasets.
- Designed a company-wide API gateway (.NET C#, AngularJS) serving 15 internal services and 3 external partners with OAuth2 and rate limiting. Deployed on AWS Elastic Beanstalk with blue-green deployments.

### **Software Engineer**
**Maloft Pte Ltd**
*Jul 2012 – Apr 2015*

- Architected automated trading systems managing $5M+ daily volume across global sports markets with sub-second order execution. Built distributed C# applications with Reactive Extensions for real-time event processing across 10+ concurrent markets.

### **Software Engineer**
**Ardmore Park Capital**
*Jan 2010 – Jun 2012*

- Built .NET WPF trading applications with Bloomberg Terminal API integration at a merger arbitrage hedge fund ($200M+ AUM). Developed portfolio exposure calculators and deal-spread tracking dashboards used daily by the trading desk.


## **Education**

- **University of Wollongong** — *Bachelor of Computer Science, Distinction*
  Dean's List · Focus in Distributed Systems and Software Engineering

- **Temasek Polytechnic** — *Diploma in Information Technology*

## **Community & Technical Writing**

- Led the Platform Engineering Guild (~80 engineers, cross-team monthly forum) — facilitated architecture reviews, shared postmortems, and drove ADR adoption across 12 platform teams.
- Authored internal blog series on Kafka operations and platform engineering patterns, referenced by 200+ engineers.
- Speaker at Singapore DevOps meetups on Kubernetes platform operations and observability at scale.
- Active contributor to internal open-source Terraform module library (200+ production consumers).
