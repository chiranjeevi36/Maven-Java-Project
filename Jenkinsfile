pipeline {
    agent { label 'build-server'}

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "maven38"
    }

    stages {
        stage('Prepare-Workspace') {
            steps {
                // Get some code from a GitHub repository
                git credentialsId: 'github-server-credentials', url: 'https://github.com/chiranjeevi36/Maven-Java-Project.git'    
            }  
        }
    }
}
