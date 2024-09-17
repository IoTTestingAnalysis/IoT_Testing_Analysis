# Repository Data Overview

This repository contains datasets and results related to our empirical analysis of unit testing practices across open-source IoT software projects. Below is a breakdown of the contents organized by each research question (RQ):

## Test Identification: Repository Data

- **Repos_Java.csv, Repos_JS.csv, Repos_Python.csv**: These files contain data on the 824 open-source projects analyzed, including various metadata for projects written in Java, JavaScript, and Python.
- **Repos_WithTest.csv**: This file lists the 317 projects that include unit tests.

## RQ1: Coverage & Mutation Score

- **Coverage.csv**: Includes statement coverage and branch coverage data for 37 projects, along with the commit IDs used to obtain the coverage data and notes for reproducing these results using a Docker image.

- **Mutation.csv**: Includes mutation score for 28 projects.

## RQ2: Open Coding of Uncovered Code Segments

- **Final_Results_RQ2.csv**: Contains the results of open coding analysis on uncovered code segments.
- **OpenCoding Folder**: Includes detailed records from two authors involved in the open coding process.

## RQ3: Mock Object Analysis

- **Final_Results_RQ3.csv**: Contains the results of open coding analysis of mock objects used in the projects.
- **Mock_FrameWork_List.csv**: Lists all the mocking frameworks identified in our dataset.
- **OpenCoding Folder**: Contains records from two authors, similar to RQ3.

## Additional Resources

- **Docker Images**: For replicating the coverage data and other test results, refer to the specific Docker images as described in the `Coverage.csv` file.

### Loading and Running Docker Containers

To load and run the Docker image, follow these steps:

1. **Download the Docker Image**:
   Download the Docker image from the [link](https://mega.nz/file/AHskCKpL#oTOENE_4jDZ67p80bcqhCVOh-ON-wurF36Wc5wTQHWU).

2. **Load the Docker Image**:
   Load the Docker image into your local Docker instance using the following command:
   ```bash
   docker load < /path/to/image.tar

3. **Run the Docker Container**:
  To run the Docker container with necessary privileges and network settings, use the following command:
  ```bash
  docker run --privileged=true --net="host" --cap-add=NET_ADMIN -v /var/run/docker.sock.raw:/var/run/docker.sock -it <image_name> bash

