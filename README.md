# lambda-layers
Various useful lambda layers for building with AWS SAM

## To create an AWS SDK layer:
1. First, clone this GitHub repo. From a terminal window (e.g. in Cloud9), execute:
```
git clone https://github.com/katjes733/lambda-layers
cd ./lambda-layers
```
2. Install the requirements.txt contents into the python (or any other runtime name) subfolder under the layer:
```
pip install -r requirements.txt -t ./layer/python
```
3. Next, deploy the AWS SAM template to create the layer:
```
sam deploy --guided
```
   - For the Stack name, enter a suitable name. Enter your preferred AWS Region and accept the other defaults.