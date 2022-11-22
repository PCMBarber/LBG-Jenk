pipeline {
    agent any
    stages {
        stage('Run Script') {
            steps {
                sh '''
                chmod +x helloWorld.sh
                ./helloWorld.sh Hi
                '''
            }
        }
        stage('Archive Cowsay') {
            steps {
                sh '''
                ssh -i "./.ssh/jenk-key" jenkins@34.130.245.1 << EOF
                touch jenkins-machine-was-errr
                EOF
                '''
            }
        }
    }
}

