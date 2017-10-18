pipeline {
    agent { node { label 'test_slave' } }
    stages {
        stage('Build') {
            steps {
                sh 'git clone https://github.com/midori15432/testMeaninglessCProject.git || (cd testMeaninglessCProject && git pull origin master)'
                sh 'gcc testMeaninglessCProject/a.c'
            }
        }
        stage('List') {
            steps {
                sh 'ls -l'
            }
        }
    }
}
