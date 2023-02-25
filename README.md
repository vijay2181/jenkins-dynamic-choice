# jenkins-dynamic-choice

- make sure jenkins user have necessary permissions to execute python script
- i have added files in /var/lib/jenkins location
- copy and paste the Jenkinsfile in pipeline job in Groovy sandbox
- when press 'build with parameters' button for the job, the python code will be executed in background and output will be sent to outpu.txt file and this output will be populated as list of choice paramters dynamically
