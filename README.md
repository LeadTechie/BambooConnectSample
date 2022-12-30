# BambooConnectSample

A sample project that uses BambooConnect

See https://github.com/LeadTechie/BambooConnect for full details

This project uses the BambooConnect library. It links to a specific test JIRA project and Google Sheet.

- It Extracts data from both
- It Transform data from each set and does a reconciliation
- It Loads the data with the updates to a Google Sheet

Effectively it runs the end to end test that the BambooConnect project contains from outside of the project to show how to use the BambooConnect project

# Detailed Setup

Setup environmental variables for Google and JIRA as per:
https://github.com/LeadTechie/BambooConnect#readme

### Python Environment Manager - Install Conda:  
- Install - [https://docs.conda.io/en/latest/miniconda.html](https://docs.conda.io/en/latest/miniconda.html)  
[https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html)  
- Update [https://www.geeksforgeeks.org/set-up-virtual-environment-for-python-using-anaconda/](https://www.geeksforgeeks.org/set-up-virtual-environment-for-python-using-anaconda/)  
Set version 3.9.12  

```
conda create -n python3-9-12 python=3.9.12 anaconda  
conda activate python3-9-12  
```

### To Run Project
```
pip install bamboo-connect

python bambooconnectsample.py
```

### To Run Project (if you wish to edit/update/extend BambooConnect project at stame time)

```
pip install -e ../BambooConnect
```

Checkout the BambooConnect project in the neighbouring directory. This allows you to directly edit the main BambooConnect project at the same time.
