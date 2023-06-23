pipeline {
    agent any

    stages {
        stage('Run playbook') {
            steps {
                script {
                    sh '''
                        ansible-playbook -b -i invent.ini nginx.yml
                    '''
                }
            }
        }
    }
}

