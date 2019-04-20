pipeline {
    agent any
    stages {
        stage('First_Build') {
            steps {
                sh 'echo "Hello World"'
            }
        }
        stage('Second_Build') {
            steps {
                 sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                    pwd
                '''
            }
        }
        stage('Third_And_Final_Build') {
            steps {
                sh '''
                echo "Ubuntu Version as below"
                lsb_release -a|grep -i release
                '''
            }
        }
    }
}
