pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/alexGobletRomano/jenkins_TP1"
            }
        }
        stage('build') {
            steps {
                sh "cd jenkins_TP1/ && javac Main.java"
            }
        }
        stage('run') {
            steps {
                sh "cd jenkins_TP1/ && java Main"
            }
        }
    }
}
