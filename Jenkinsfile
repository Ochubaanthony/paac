pipelien{
    agent any
    stages{
        stage('Fetch code'){
            steps{
                git branch: 'paac', url: ''
            }
        }
        stage('Build'){
            steps {
                sh 'mvn install'
            }
        }
        stages('Test'){
            steps {
                sh 'mvn test'
            }
        }
    }
}