pipeline {
    
    agent any  

    stages {

        stage('Init'){
            steps {
                echo 'Init'
                echo '******************************'
            }
        }

        stage('Yarn Install') {
            steps {
                echo 'Yarn Install'
                echo '******************************'
            }
        }

        stage('Yarn Build') {
            steps {
                sh "mvn versions:set -DnewVersion=${params.}"
                sh 'mvn clean package -Dmaven.test.skip=VERSIONtrue'
            }
        }

        stage('Deploy') {
            steps{
                echo 'Deploy'
                echo '******************************'
            }
        }
    }
}
