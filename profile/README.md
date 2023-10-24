# netUnicorn project

## Description

This is an organization that contains public code for the netUnicorn project.

netUnicorn is a platform for building and running data pipelines on different nodes for data collection experiments. It allows users to express arbitrary Python-based tasks and pipelines and assign them to particular nodes of different architectures.

This platform is a pipeline-based platform (like Apache Airflow or CI/CD solutions), but instead optimizes the following:
-  the ability to use different infrastructures via specific connectors (e.g., SaltStack-based, Azure Container Instances, Mininet, etc.)
-  the short time between tasks
-  work under the conditions of an unstable network
-  reproducibility and easy sharing of tasks and pipelines

## How to use

To use netUnicorn, its director services should be deployed on organization premises and connected to available network infrastructures.

- Administrators of the platform should deploy the platform and ensure the network infrastructure connection and availability of the endpoints.
- Platform users should install `netunicorn-client` and (optionally, but highly recommended) `netunicorn-library` Python packages and obtain credentials (username, password, connection endpoint) from Administrators.

Please, see the documentation of the `netunicorn` repository for further details.

## Repositories

This organization contains the next repositories:
- `netunicorn` - this is the main repository of the system, including base, client, and directory services source code.
- `netunicorn-library` - this is the repository that contains all public implementations of different tasks and pipelines. Pull Requests with your implementations are welcome!
- `netunicorn-connector-...` - these repositories contain netUnicorn connector implementation for different network infrastructure providers, such as Kubernetes, AWS, SaltStack, etc.'
- `netunicorn-search` - this is a supplementary repository, containing artifacts for the research paper presenting netUnicorn.

## Cite us

```Roman Beltiukov, Wenbo Guo, Arpit Gupta, and Walter Willinger. 2023. In Search of netUnicorn: A Data-Collection Platform to Develop Generalizable ML Models for Network Security Problems. In Proceedings of the 2023 ACM SIGSAC Conference on Computer and Communications Security (CCS ’23), November 26–30, 2023, Copenhagen, Denmark. ACM, New York, NY, USA, 15 pages. https://doi.org/10.1145/3576915.3623075```

See also the extended version of the paper: https://arxiv.org/abs/2306.08853

INFO: BibTeX citations will be available later