pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
               checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://Shahnoor_Arshid@bitbucket.org/shahnoor_arshid/testing_repo.git']])
            }
        }
        stage ('Build'){
            steps {
                git 'https://Shahnoor_Arshid@bitbucket.org/shahnoor_arshid/testing_repo.git' 
       
            }
        }
  	stage ('run'){
            steps { 
               sh 'cp index.html /var/www/html/'

            }
        }


   
    }
}
