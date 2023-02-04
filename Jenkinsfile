pipeline {
    agent none
    stages {
        stage('KVM - Delete exited containers') {
            agent {
                label "KVMDEBTEST01"
            }
            steps {
                sh"""
                sudo su cblock -c "source ~/.profile; docker_gentoo" || exit 0
                """
            }
        }
        stage('PROD - Delete exited containers') {
            agent {
                label "HQDEBPROD01"
            }
            steps {
                sh"""
                sudo su cblock -c "source ~/.profile; docker_gentoo" || exit 0
                """
            }
        }
        stage('Dev - Delete exited containers') {
            agent {
                label "HQDEBDEV01"
            }
            steps {
                sh"""
                sudo su cblock -c "source ~/.profile; docker_gentoo" || exit 0
                """
            }
        }
        stage('DELL - Delete exited containers') {
            agent {
                label "HQDEBDELL01"
            }
            steps {
                sh"""
                sudo su cblock -c "source ~/.profile; docker_gentoo" || exit 0
                """
            }
        }
        stage('Lenovo - Delete exited containers') {
            agent {
                label "HQDEBLENOVO01"
            }
            steps {
                sh"""
                sudo su cblock -c "source ~/.profile; docker_gentoo" || exit 0
                """
            }
        }
    }
}
