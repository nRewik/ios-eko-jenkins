pipeline {
    agent {
        node {
            label 'macos'
        }
    }
    options { 
        disableConcurrentBuilds() 
    }
    environment {
        // AWS_ACCESS_KEY_ID     = credentials('jenkins-aws-secret-key-id')
        // AWS_SECRET_ACCESS_KEY = credentials('jenkins-aws-secret-access-key')
    }
    stages {
        stage('Test Build') {
            steps {
                echo 'Build client ${params.client_name}'
            }
        }
    }
}
