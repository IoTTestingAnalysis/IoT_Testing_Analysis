# Repository Data Overview

This repository contains datasets and results related to our empirical analysis of unit testing practices across open-source IoT software projects. Below is a breakdown of the contents organized by each research question (RQ):

## RQ1: Repository Data

- **Repos_Java.csv, Repos_JS.csv, Repos_Python.csv**: These files contain data on the 824 open-source projects analyzed, including various metadata for projects written in Java, JavaScript, and Python.
- **Repos_WithTest.csv**: This file lists the 317 projects that include unit tests.

## RQ2: Coverage Data

- **Coverage.csv**: Includes statement coverage and branch coverage data for 37 projects, along with the commit IDs used to obtain the coverage data and notes for reproducing these results using a Docker image.

## RQ3: Open Coding of Uncovered Code Segments

- **Final_Results_RQ3.csv**: Contains the results of open coding analysis on uncovered code segments.
- **OpenCoding Folder**: Includes detailed records from two authors involved in the open coding process.

## RQ4: Mock Object Analysis

- **Final_Results_RQ4.csv**: Contains the results of open coding analysis of mock objects used in the projects.
- **Mock_FrameWork_List.csv**: Lists all the mocking frameworks identified in our dataset.
- **OpenCoding Folder**: Contains records from two authors, similar to RQ3.

## Additional Resources

- **Docker Images**: For replicating the coverage data and other test results, refer to the specific Docker images as described in the `Coverage.csv` file.
