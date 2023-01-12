pipeline {
    agent none
    stages {
        stage('Compile') {
            agent any
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
            agent any
            steps {
               echo "Package  job"
            }
        }
        stage('commit') {
            agent any
            steps {
               echo "commit  job"
            }
        }
        stage('play') {
            agent any
            steps {
               echo "play  job"
            }
        }
        stage('plawrongy') {
            agent any
            steps {
               echo "playwrong  job"
            }
        }
        }
}