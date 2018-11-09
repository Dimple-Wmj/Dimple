// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
   
    stages {
        stage('Build') {    //stage('Build')
            steps {
                echo 'Building..'
                sh 'echo "Hello Jenkins > test.txt'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
