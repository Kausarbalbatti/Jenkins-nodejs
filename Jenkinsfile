pipeline{
    agent any
    stages{
        stage("Clone repository")
        {
            steps
            {
                git branch:'main',url:'https://github.com/Kausarbalbatti/Jenkins-nodejs.git'
            }
        }
        //Node js clone repository done Q12


        stage("Install dependencies")
        {
            steps{
                sh 'npm install'
            }
        }
        // stage("Testing")
        // {
        //     steps{
        //         sh 'npm test'
        //     }
        // }
        stage("Start the app")
        {
            input{
                message'Do you want to start?'
                ok "Click on OK"
                submitter 'Bushra'
            }
          steps{
           sh 'npm start'
          }
        }
    }
}