pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 echo 'Build by CS280 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test by CS280 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by CS280 successful'
            }
        }
    }

    post {
        always {
            if (currentBuild.result == 'FAILURE') {
                echo 'Pipeline Failed'
            }
        }
    }
}
