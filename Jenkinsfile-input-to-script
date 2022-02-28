pipeline {
    agent any
    stages {
        stage('tryinput') {
            steps {
                sh 'ls -la'
                retry(3) {
                    sh './test-input-script.sh'
                }
                sh 'ls -la'
            }
        
        }
    }
}
