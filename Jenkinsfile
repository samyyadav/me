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
                mkdir -p /var/www/html/my_project # Change to your target directory
                cp -r * /var/www/html/my_project
                '''
            }
        }
    }
}
