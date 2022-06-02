pipeline {
    agent any
    stages {
        // ("Build" stage omitted)
        stage('Test') {
            steps {
                // (Steps omitted)
                // ("junit" step moved to "post" section)
            }
        }
    }
    post {
        always {
            // Report test results
            junit 'target/surefire-reports/*.xml'
        }
    }
}
