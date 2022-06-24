# Google Cloud associate cloud engineer notes

**Table of Contents**
1. [GCP Fundamentals](#gcp-fundamentals)
2. [Setting up a cloud solution environment](#setting-up-a-cloud-solution-environment)
    - [Setting up cloud projects and accounts](#setting-up-cloud-projects-and-accounts)

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
**Creating Projects**
High level organization called resource manager hierarchy:
    - Organization >> Folder >> Projects >> Resources
    - More info [here](https://cloud.google.com/resource-manager/docs/cloud-platform-resource-hierarchy)

- Project IDs are globally unique
- Billing accounts are associated to projects same as resources
- Shut down a project deletes everything (resources) in the project

**Assign users to predefined IAM roles within a project**
- Users:
    - Can get roles assigned
    - Users are created through IAM
- Roles = collection of permissions
- GCP has predefined roles
- Always apply the least permissions to users (only the ones needed)

**Manage users in cloud identity**

Cloud Identty:
- Google Account
    - Username and password (gmail account)
- Service Principal
    - Used for applications
    - Resources are attach to a service account
    - Provides access to application running in resources (such as compute engine) (example: an application trying to access BigQuery)
    - Can attach roles to service accounts
- G-Suit Domain
    - Now know as google workspace
    - Users in workspaces can access to google cloud
    - Allow to have custom domains
- Cloud Identity Domain [URL](https://cloud.google.com/identity#section-1)
    -   Allow custom domains that are not from workspace (g-suit)
- Google group
    -   Can create a google group and add users, which the members of a group can get access permissions
    - Roles can be assigned to the group it self

**Enabling APIs within projects**
