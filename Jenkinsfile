pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                label 'jenkins-jx-base'
            }
            steps {
                echo 'Build..'
            }
        }
        stage('Test on Linux') {
            agent {
                label 'jenkins-terraform'
            }
            steps {
                echo 'Test on Linux..'
            }
        }
        stage('Test on Windows') {
            agent {
                label 'jenkins-maven'
            }
            steps {
                echo 'Test on Windows..'
            }
        }
    }
}