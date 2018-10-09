pipeline {
    agent any
    stages {
        stage('Docker Build') {
            dir('storage') {
                steps {
                    sh "oc start-build storage --follow --from-file=./Dockerfile"
                }
            }
        }
    }
}
