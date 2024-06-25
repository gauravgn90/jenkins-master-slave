Generate SSH key

- ssh-keygen -t rsa -f jenkins-agent
- cat jenkins-agent
- Add this key in Jenkins credentials and do not use the username(as of now)
- cat jenkins-agent.pub
- Copy the pub key
- Paste in docker-compose file
- Now add a new agent in Jenkins
- Add /home/jenkins/agent in the remote root directory
- Select 'use this node as much as possible'
- Enter the name of the host  in the docker-compose.yml file hostname is jenkins-agent2
- Host key verification will be a nonverification strategy
- Select Advanced option
- port value will be 22
- java path value will be /opt/java/openjdk/bin/java
- Set connection time-out settings
- set retires setting
- set wait  between retries

- Set up Completed check agent logs once you save the agent configs.

For further reference use the below URL

https://www.cloudbees.com/blog/how-to-install-and-run-jenkins-with-docker-compose
