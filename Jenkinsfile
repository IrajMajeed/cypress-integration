pipeline {
    agent any
    stages{
      stage('Run Cypress Tests') {
            steps {
                script { 

                    sh "sudo chown -R 1000:1000 '/home/jenkins/.npm'"
                    sh "npm cache clean –force"
                    sh "npm ci "
                    sh "sudo npm run cypress-test"
                    
                    }  
                }
      } 
    
    }
}


