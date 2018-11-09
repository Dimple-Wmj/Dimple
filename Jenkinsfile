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
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                echo "
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
