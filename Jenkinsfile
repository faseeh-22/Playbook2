pipeline {
    agent any

    stages {
        stage('Clone repository') {
            steps {
                git credentialsId: 'git', url: 'https://github.com/faseeh-22/Playbook2.git'
            }
        }

        stage('Run playbook') {
            steps {
                sh 'ansible-playbook -b -i invent.ini nginx.yml'
            }
        }
    }
}
