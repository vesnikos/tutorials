# Http Communication with Requests

## Learning Objectives

### At the end of this tutorial, you will be able to:
1. Install the `requests` library
1. Make HTTP requests using the `requests` library
1. Use the `requests` library to make a GET request
1. Use the `requests` library to make a POST request
1. Parse JSON responses


## Introduction


### Requests

The `requests` library is a simple and elegant HTTP library for Python. It is designed to make HTTP requests simpler and more human-friendly. The `requests` library is built on top of the `urllib3` library, which is a very powerful HTTP library.

> Note: There are different protocols besides HTTP that can be used to communicate over the internet. Such protocols include FTP, SSH, and SMTP. The `requests` library only supports HTTP.

#### Installation

To install the `requests` library, run the following command in your terminal:

```console
$ pip install requests
```

#### Basic Usage

After installing the `requests` library you will be able to import it to your python file:

```python
import requests

response = requests.get('http://www.google.com')
print(response.status_code)
# <Response [200]>
```

### Pages

1. [requests-intro](./notebooks/requests-intro.ipynb)
1. [requests-status-codes](./notebooks/status-codes.ipynb)
1. [requests-json](./notebooks/requests-json.ipynb)
1. [requests-async](./notebooks/requests-async.ipynb)

