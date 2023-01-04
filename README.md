# create-pdf-on-lambda

## For local

1. Install wkhtmltopdf

```sh
sudo apt install -y wkhtmltopdf
```

2. Enable the code for local env

Uncomment the below code in handler.py.

```python
# wkhtmltopdf_path = '/usr/local/bin/wkhtmltopdf'
```

3. Execute pip install -r requirements.txt

4. Run handler.py on local


## For AWS Lambda

1. Download wkhtmltopdf (lambda zip) from [official page](https://wkhtmltopdf.org/downloads.html)

2. Upload the zip you downloaded as AWS Lambda Layer to AWS

3. Add AWS Lambda Layer ARN to serverless.yml

4. Execute sls deploy

5. Run the lambda function on AWS


## Referencces

[Building a PDF Generator on AWS Lambda with Python3 and wkhtmltopdf](https://blog.richardkeller.net/building-a-pdf-generator-on-aws-lambda-with-python3-and-wkhtmltopdf/)
