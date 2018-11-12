// Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    environment {
     TEST_COMMON_CREDS = credentials('jenkins-test-common-creds')   
    }
    parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
        string(name: 'Testing', defaultValue: 'Testing', description: "Testing...")  
    }
   
    stages {
        stage('Build') {    //stage('Build')
            steps {
                echo 'Building..'
                sh 'touch text.txt && echo "Hello Jenkins" > test.txt'
            }
        }
        stage('Test') {
            environment {
                USERNAME = 'Jenkins'
                // Using returnStdout
                //CC = """{sh(
                //        returnStdout: true,
                //        script: 'echo "clang"'
                //     )}"""
                // Using returnStatus
                //EXIT_STATUS = """{sh(
                //                returnStatus: true,
                //                script: 'exit 1'
                //               )}"""   
            }
            steps {
                echo 'Testing..'
                // echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
                echo "Hi Mr. ${USERNAME}"
                echo "I said Hi Doc. ${USERNAME}"
                echo " hello Jenkins"
                // echo "Test ${TEST_COMMON_CREDS}"
                // echo "USR ${TEST_COMMON_CREDS_USR}"
                // echo "PSW ${TEST_COMMON_CREDS_PSW}"
                echo "${params.Greeting} World!"
                echo "${params.Testing} ..."
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                echo "${params.Testing} ..."
            }
        }
    }
}
