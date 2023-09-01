pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
                script {
                    def customWorkspace = '/mnt/data'
                    ws(customWorkspace) {
                        sh "cp -r index.html /var/www/html"
                        sh "chmod -R 777 /var/www/html/index.html"
                    }
                }
            }
        }
        stage('start') {
            steps {
                sh "service httpd start"
            }
        }
    }
}

