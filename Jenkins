pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                echo 'build'
            }
        }
            
            stage('test') {
            steps {
                echo 'test'
            }
        }
            stage('deploy') {
            steps {
                echo 'deploy'
            }
            
        }
    }
    
    post{
        always
        {
            emailext body: 'Mail from jenkins after running the project ', subject: 'Jenkins Test', to: 'qa.ssdtest@gmail.com'
        }
    }
    
}
