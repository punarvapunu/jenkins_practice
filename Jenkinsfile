@Library("my_library") _
pipeline{
    agent any
   
    stages{
        stage("Checkout"){
            steps{
                echo "excuting"
                script{
                def config = [
                    url: 'https://github.com/punarvapunu/maven_calculator_app-main.git',
                    branch: 'main',
                    credentialsId: 'github_token'
                

                       
                ]
                gitCheckout(config)   
                sh '''
                    pwd
                    ls -lrt 
            
                '''
                }
            }


        }

    }
}

