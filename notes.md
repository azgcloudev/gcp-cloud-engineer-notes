# Google Cloud associate cloud engineer notes

**Table of Contents**
1. [GCP Fundamentals](#gcp-fundamentals)
2. [Setting up a cloud solution environment](#setting-up-a-cloud-solution-environment)
    2.1 [Setting up cloud projects and accounts](#setting-up-cloud-projects-and-accounts)

## GCP Fundamentals
- Cloud provides elasticity
- You rent services instead of buy hardware
- GCP provides 200+ services

**Cloud Advantages**
- Take advantage of economies of scale (cloud providers get better prices to buy multiple hardware from manufactures which allows lower pricing to provide services to the clients)
- Trade Capital Expenditure (CapEx) for Operational Expenditure (OpEx)
- You do not need to guess capacity (for peak workloads)
- No need to maintain data centers
- Can go global in minutes
- On demand resources (you can release them when you do not need them)

**Google Cloud Platform (GCP)**
- Is on to the top 3 cloud providers
- Provides 200+ services
- Is a net carbon-neutral cloud (electricity used is 100% renewable energy)
- Is reliably, secure and highly performant

**Why GCP**
- Trust and security
    - Trust nothing by default
- Open cloud platform (Open API) [more info](https://cloud.google.com/open-cloud)
- Global network infrastructure [link](https://cloud.google.com/about/locations#network)
- AI Driven Cloud

### Regions and Zones

#### Regions
- Are specific geographical locations to place the data centers
- As of June 2022 GCP has 34 regions
- Advantages:
    - High availability (deploy services in multiple regions)
    - Low latency (deploy services near to your clients)
    - Global footprint (deploy services easy across the globe)
    - Adhere to regulation (example storage US customer information only in US data centers)

#### Zones

Zones provide high availability within the same region.
- Each region has at least three zones
- Increase availability and fault tolerance within the same region
- Zones are composed of one or more data centers (independant physical locations)
- Zones of a regions are connected with low latency links (fiber connections)


### GCP Services
- Computing and hosting
- Storage
- Databases
- Networking
- Big data
- Machine learning

---

## Setting up a cloud solution environment
### Setting up cloud projects and accounts
