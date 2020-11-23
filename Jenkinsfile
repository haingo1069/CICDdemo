pipeline {
    agent any 
    stages {
        stage('build1') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
        stage('test1') {
            steps {
                sh 'docker -version' 
            }
        }
        stage('deploy1') {
            steps {
                echo 'Hello world!' 
            }
        }
    }
}