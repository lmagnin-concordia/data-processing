pipeline {
    agent any
    stages {
       stage('Docker Build') {
          steps {
             dir('storage') {
                   sh "oc new-build --strategy docker --binary --name storage"
                   sh "oc start-build storage --follow --from-file=./Dockerfile"
                }
            }
        }
    }
}
