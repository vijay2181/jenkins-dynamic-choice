# jenkins-dynamic-choice

- make sure jenkins user have necessary permissions to execute python script
`chown -R jenkins:jenkins input.py output.txt`
- i have added files in /var/lib/jenkins location
- copy and paste the Jenkinsfile in pipeline job in Groovy sandbox
- when press 'build with parameters' button for the job, the python code will be executed in background and output will be sent to outpu.txt file and this output will be populated as list of choice paramters dynamically, it will ask for user input selection where, user can select option

![image](https://user-images.githubusercontent.com/66196388/221340829-11f39e2b-d88a-419a-93a3-eef7b7c6aaa0.png)


![image](https://user-images.githubusercontent.com/66196388/221340849-2d5a5d22-76ef-4b0c-8434-a290cf53f0e3.png)


![image](https://user-images.githubusercontent.com/66196388/221340867-e9fb384b-4215-433f-b83f-b5ea5d539309.png)
