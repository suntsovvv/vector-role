pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Download role from github') {
            steps {
                git 'https://github.com/suntsovvv/vector-role.git'
            }
        }
        stage('m_test') {
            steps {
                sh 'molecule test'
            }
        }
    }
}
