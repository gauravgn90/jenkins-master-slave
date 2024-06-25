Generate SSH key

- ssh-keygen -t rsa -f jenkins-agent
- cat jenkins-agent
- Add this key in jenkins credentials and do not use username(as of now)
- cat jenkins-agent.pub
- Copy the pub key
- Paste in docker compose file
- Now add new agent in jenkins
- Add /home/jenkins/agent in remote root directory
- Select 'use this node as much as possible'
- Enter name of the host  in docoker-compose.yml file host name is jenkins-agent2
- Host key verification will be non verification strategy
- Select Advanced option
- port value will be 22
- javapath value will be /opt/java/openjdk/bin/java
