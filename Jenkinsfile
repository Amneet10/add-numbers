pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                script {
                    checkout([$class: 'GitSCM',
                              branches: [[name: '*/main']], // Checkout the master branch
                              userRemoteConfigs: [[url: 'https://github.com/Amneet10/add-numbers.git']]]) // Specify your GitHub repository URL
                }
            }
        }
        
        // Add more stages for your pipeline as needed
    }
    
    // Post-build actions, notifications, etc.
}
