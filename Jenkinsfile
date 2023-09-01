pipeline {
    agent any
    stages {
        stage('stage-1') {
            steps {
                script {
                    def customWorkspace = '/mnt/data'
                    ws(customWorkspace) {
                        echo "hello this is 23Q1 branch"
                    }
                }
            }
        }
        stage('stage-2') {
            steps {
                echo "this is 23Q1 branch"
            }
        }
    }
}

