# Setup

Here below a brief overview of the setup realized.

## Architecture

The architecture is composed of 5 components:
  
  - Storage
  - Processing
  - Interfaces
  - CI/CD
  - Containers
  
Storage:
  - data is stored on hdfs
  - documents are indexed on elastic search
  - code is stored on git and managed by gitlab
  
Processing:
  - distributed: spark (python API)
  - non distributed: scikit-learn, pandas (python)

Interfaces:
  - services and custom UI via APIs in Flask and Vue.js apps
  - JDBC of parquet tables via spark jdbc thrift server
  - JupyterHub: ETL and Data Science Notebooks
  - Kibana for elastic search exploration and dashboards
  - BI analtics with Redash and Power BI

CI/CD:
  - Scheduling and Execution via Gitlab CI

Containers:
  - Management, Deployment, Scaling via Kubernetes (To do)

Provisioning:
  - Ansible
  - Kubernetes

## Getting Started

  - Data
     - hierarchy
     - conventions     

  - Ingest: 
     - jupyter
     - datalabframework,
     - spark
     - git / gitlab
     - gitlab ci/cd

  - ETL: 
     - jupyter
     - datalabframework,
     - spark
     - git / gitlab
     - gitlab ci/cd

  - Reporting: 
     - jupyter
     - datalabframework,
     - spark
     - git / gitlab
     - gitlab ci/cd
     - Templating

  - Data Science: 
     - jupyter
     - datalabframework
     - spark
     - elastic
     - elastictools
     - git, gitlab
     - Flask Restful API
  
  - BI and Analytics
     - Kibana
     - BI Tools: Redash, Power BI, Tableau, etc
  
  - Provisioning
    - overview of system:
      - services running
      - Managing APIs
      - Managing Batch flows
      - Managing Streaming
    - boostrapping

