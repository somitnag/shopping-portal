pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('complie'){
            steps{
                echo 'this is the compile job'
                sh 'npm install'
                 }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                 }
        }
        stage('package'){
            steps{
                echo 'this is the third job'
                sh 'npm run package'
                 }
        }
    }
    
    post{
        always{
            echo 'this is my dojo pipeline.'
        }
        
    }
    
}
