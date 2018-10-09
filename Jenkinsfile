pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                sh 'oc version'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
