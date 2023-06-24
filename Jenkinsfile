pipeline{

    agent any

    tools{
       nodejs 'nodejs' 
    }   

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('Test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('Package'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
