pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
               echo "Compile  job"
            }
        }   
        stage('Unit Test') {
            agent label{'linux-slave'}
            steps {
               echo "UnitTest  job"
            }
        }
        stage('Package') {
            steps {
               echo "Package  job"
            }
        }
        stage('commit') {
            steps {
               echo "commit  job"
            }
        }
        stage('play') {
            steps {
               echo "play  job"
            }
        }
        stage('plawrongy') {
            steps {
               echo "playwrong  job"
            }
        }
        }
}