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
                git version: "${params.VERSION}"
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
