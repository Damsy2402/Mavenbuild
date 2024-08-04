pipeline {
    
    agent any
    
    stages {
        
        stage('build') {
            
            steps {
                
                echo 'hello'
                
            }
        }
        
        stage('test') {
            
            steps {
               
                echo 'welcome'
            }
        }
        
        stage('deploy') {
            
            steps {
                
                echo 'all'
            }
        }
    }
    post {
        always {
            emailext body: 'Execution status of testpipeline', subject: 'Pipeline status', to: 'srinivas.srinu83@gmail.com'
        }
    }
}