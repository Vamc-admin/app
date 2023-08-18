pipeline {

    agent any

    stages{

        stage('Git checkout'){

            steps{
                git 'https://github.com/Vamc-admin/app.git'
            }
        }

        stage("unit test"){

            steps{
                
                sh 'mvn test'
            }
        }
    }
}
