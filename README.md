# Example for redeploy alias fail: AWS::Lambda::Version is not supported

## Steps

1. export DEPLOY_TAG=build-100
1. node ./node_modules/serverless/bin/serverless deploy --alias dev (work)
1. export DEPLOY_TAG=build-101
1. node ./node_modules/serverless/bin/serverless deploy --alias uat (work)
1. export DEPLOY_TAG=build-102
1. node ./node_modules/serverless/bin/serverless deploy --alias uat (fail)