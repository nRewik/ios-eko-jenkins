pipeline {
    agent {
        node {
            label 'macos'
        }
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
