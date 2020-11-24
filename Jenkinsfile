pipeline {
    agent any 
    stages {
        stage('build') {
            steps {
                sh 'echo "Start building docker container"'
                sh '''
                    docker build -t rndevapp/mytest:0.1.0 -f Dockerfile .
                    docker image ls
                '''
            }
        }
        stage('test') {
            steps {
                sh 'echo start testing' 
            }
        }
        stage('push to docker hub') {
            steps {
                sh '''
                docker login -u rndevapp -p haingo0858
                docker push rndevapp/mytest:0.1.0
                '''
            }
        }
    }
}