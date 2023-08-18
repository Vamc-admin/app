pipeline {

    agent any

    stages{

        stage('Git checkout'){

            steps{
                git 'https://github.com/Vamc-admin/app.git'
            }
        }

        stage('unit test'){

            steps{
                
                sh 'mvn test'
            }
        }
        stage('Integration testing'){

            steps{

                sh 'mvn verify -DskipUnitTests'
            }
        }
        stage('Maven Build'){

            steps{

                sh 'mvn clean install'
            }
        }
    }
}
