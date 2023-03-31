pipeline {
    agent any

    stages {
        stage('Cloning') {
            steps {
                git url: 'https://github.com/clem-kay/jenkins_aws.git', branch: 'main'
               
            }
        }
          stage('Building Image') {
            steps {
               sh 'docker build -t clem/clem_webserver:latest .'
               
            }
        }
    }
}
