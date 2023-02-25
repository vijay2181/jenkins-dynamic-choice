pipeline {
    agent any

    stages {
        stage('Run Python Script') {
            steps {
                sh 'python3 /var/lib/jenkins/input.py > /var/lib/jenkins/output.txt'
            }
        }
        stage('Capture Script Output') {
            steps {
                script {
                    env.SCRIPT_OPTIONS = readFile('/var/lib/jenkins/output.txt').trim().split('\n').join('\n')
                }
            }
        }
        stage('Run Pipeline with Parameters') {
            steps {
                script {
                    def userInput = input message: 'Select an option:',
                        parameters: [choice(name: 'SCRIPT_OPTION', choices: env.SCRIPT_OPTIONS)]
                    echo "You selected: ${userInput}"
                }
            }
        }
    }
}
