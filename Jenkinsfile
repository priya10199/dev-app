pipeline {
    agent any
    stages {
        stage('stage-1') {
            steps {
                script {
                    def customWorkspace = '/mnt/data'
                    ws(customWorkspace) {
                        sh "mkdir TEST"
                    }
                }
            }
        }
        stage('stage-2') {
            steps {
                sh "mkdir folder"
            }
        }
    }
}

