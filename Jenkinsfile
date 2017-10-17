pipeline {
    agent any

    stages {
        stage('Copy paste detection') {
            steps {
                sh 'cp ./* /var/www/html/'
            }
        }
        stage('cleanup') {
            // Recursively delete all files and folders in the workspace
            // using the built-in pipeline command
            deleteDir()
        }
    }
}