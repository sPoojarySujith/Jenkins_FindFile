pipeline {
    agent any
    stages {
        stage('Search for file') {
            steps {
                sh 'find $WORKSPACE -name "cucumber.json"'
            }
        }
    }
}
