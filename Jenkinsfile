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
                /usr/games/cowsay "Good Job Class" > wew.txt
                '''
            }
        }
    }
}

