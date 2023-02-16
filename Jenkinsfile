pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ error -o PES2UG20CS372-1 try.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS372-1'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
