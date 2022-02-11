# lambda-layers
Various useful lambda layers for building with AWS SAM

## To create an AWS SDK layer:
1. First, clone this GitHub repo. From a terminal window (e.g. in Cloud9), execute:
```
git clone https://github.com/katjes733/lambda-layers
cd ./lambda-layers
```
2. Navigate to the corresponding layer sub directory (e.g. jwt):
```
cd ./jwt
```
3. Build with a lambda like container:
```
sam build --use-container
```
4. Next, deploy the AWS SAM template to create the layer:
```
sam deploy --guided
```
   - For the Stack name, enter a suitable name. Enter your preferred AWS Region and accept the other defaults.
   - For future builds, the parameter --guided may be omitted if parameters dont change:
   ```
    sam deploy
    ```