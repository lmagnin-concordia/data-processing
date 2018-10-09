pipeline {
    agent any
    stages {
       stage('Docker Build') {
          steps {
             dir('storage') {
                   sh "oc new-build --name storage"
                   sh "oc start-build storage --follow --from-file=./Dockerfile"
                }
            }
        }
    }
}
