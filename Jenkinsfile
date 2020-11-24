pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                sh 'echo "Start building docker container"'
                sh '''
                    docker build -f Dockerfile .
                    docker image ls
                '''
            }
        }
        stage('test') {
            steps {
                sh 'echo start testing' 
            }
        }
        stage('deploy') {
            steps {
                echo 'Hello world!' 
            }
        }
    }
}