## Introduction
Integration testing is a critical part of software testing that focuses on the interaction between different components of a software application. In this project, we demonstrate how to use the Requests library and Python to perform integration tests on a REST API. We provide a simple example that sends a GET request to an API, verifies the response status code, and verifies that the response contains the expected data. This project is useful for software developers and testers who want to ensure that their application's components are functioning correctly when integrated together.

## Requirements
To use this project, you'll need the following software installed on your system:

- Python 3.x
- pip (Python package manager)
- Requests library

## Installation
1. Install the Requests library for Python by running the following command:
```
pip install requests
```

## Usage
1. Open a text editor or IDE of your choice and create a new Python script.

2. Import the necessary modules in your Python script:
```python
import requests
```

3. Send a GET request to the API using the requests.get() method:
```python
response = requests.get("http://api.example.com/resources")
```

4. Verify that the response has a status code of 200 (OK) using the response.status_code attribute:
```python
assert response.status_code == 200
```

5. Verify that the response contains the expected data using the response.json() method and comparing it to the expected data:
```python
assert response.json() == {"resources": [{"id": 1, "name": "Resource 1"},
                                        {"id": 2, "name": "Resource 2"}]}
```

## Conclusion
With this project, you can write integration tests that ensure your application's components are functioning correctly when integrated together. You can customize these tests to include more complex scenarios and test cases, depending on your application's requirements. If you have any questions or feedback, please let us know!