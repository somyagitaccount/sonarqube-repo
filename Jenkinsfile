#!groovy
pipeline {
  agent any
//   environment {
//     AWS_ACCESS_KEY_ID = credentials('AWS_ACCESS_KEY_ID')
//     AWS_SECRET_ACCESS_KEY = credentials('AWS_SECRET_KEY')

//   }
  stages {
        stage('checkout') {
            steps {

                git branch: 'main', url: 'https://github.com/somyagitaccount/sonarqube-repo.git'

                  }
              }
        

        stage('run ansible playbook-install-packages such as sonarquebe') 
            {
            steps {

                sh "ansible-playbook main.yml -i hosts --user ubuntu "
            }
        }

    }
}