

my-chatgpt
docker login -u koala95271 registry.cn-shenzhen.aliyuncs.com -p jijiwaiwai123...
docker build . -t $PROJECT_NAME - docker tag $PROJECT_NAME $REGISTRY_URL/$PROJECT_NAME:$CI_COMMIT_REF_NAME
docker tag $PROJECT_NAME $REGISTRY_URL/$PROJECT_NAME:latest
docker push $REGISTRY_URL/$PROJECT_NAME:$CI_COMMIT_REF_NAME
docker push $REGISTRY_URL/$PROJECT_NAME:latest


registry.cn-shenzhen.aliyuncs.com/koala9527/my-chatgpt-web:v1.0.0