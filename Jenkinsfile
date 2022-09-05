pipeline{
    agent any
    stages{
        stage('Fetch code'){
            steps{
                git branch: 'paac', url: 'https://github.com/devopshydclub/vprofile-project' //if you want to fetch the step from pipleline
            }
        }
        stage('Build'){
            steps{
                sh 'mvn install'
            }
        }
        stage('Test'){
            steps{
                sh 'mvn test'
            }
        }
    }
}