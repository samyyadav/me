pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out the code...'
                checkout scm // Ensures the code from the repository is checked out
            }
        }

        stage('Build') {
            steps {
                echo 'No build required for HTML. Skipping...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying HTML files...'
                // Example: Copying files to a remote server (adjust to your needs)
                sh '''
                ls -la
                mkdir -p ~/html/my_project
                cp -r * ~/html/my_project
                '''
            }
        }
    }
}
