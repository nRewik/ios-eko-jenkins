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
    parameters {
        string(name: 'client_name', defaultValue: 'eko', description: 'The client folder name, used as config for building')
    }
    stages {
        stage('Test Build') {
            steps {
                echo 'Build client ${params.client_name}'
            }
        }
    }
}
