pipeline {
    agent any
    stages{
      stage('Post Deployment Tests Cypress') {
            steps {
                script { 

                    sh "sudo chown -R 1000:1000 '/home/jenkins/.npm'"
                    sh "npm cache clean –force"
                    sh "npm ci "
                    sh "sudo npm run test"
                    
                    }  
                }
      } 
    
    }
}


