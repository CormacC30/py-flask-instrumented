# py-flask-instrumented

## A simple example of a python application, instrumented with client_python for prometheus

### What does this do?
This is simple python-flask app that returns a 200 response code when HTTP request is made to the '/health' endpoint

"client_python" is used to expose metrics that can be scraped by Prometheus.

The target endpoint for prometheus is '/metrics'

### Instructions

1. Download and install dependencies

```
git clone https://github.com/CormacC30/py-flask-instrumented.git
cd py-flask-instrumented
pip install flask
pip install prometheus-client
```

2. Run application and test

```
python3 healthy-instrumented.py
```

Browse to `http://localhost:8080/health' 

3. Configure prometheus target to scrape metrics