pipeline {
    agent { node { label 'Agent_1' } }
    stages {
        stage('Install depdencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Unit test') {
            steps {
                echo "unit testing is done here"
            }
        }
        //sonar-scanner command expect sonar-project.properties should be available
        // stage('Sonar Scan') {
        //     steps {
        //         sh 'ls -ltr'
        //         sh 'sonar-scanner'
        //     }
        // }
        stage('Build') {
            steps {
                sh 'ls -ltr'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deployment"
            }
        }
    }
}