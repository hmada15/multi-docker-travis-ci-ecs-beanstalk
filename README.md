## Multi-docker app with travis-ci deployed on AWS Elastic Beanstalk backed by AWS ECS
The application includes front-end ReactJs, back-end NodeJs, worker NodeJs, Postgres and Redis containers
 
#### How it work
On every push or merge to github, travis-ci pull the code, build the docker images, push them to docker hub than deploy the app to Elastic Beanstalk, Elastic Beanstalk create the task definition in ECS and ECS pull the images and run them.
