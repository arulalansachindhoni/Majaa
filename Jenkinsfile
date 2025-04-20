pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build the Application'
            }
        }
         stage('Test') {
            steps {
                echo 'Test the Application'
            }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy the Application'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Summary', subject: 'Pipeline Status', to: '2000113907@hexaware.com'
        }
    }
}
