pipeline {

    agent { 

        node {

            label 'docker-agent'

            }

      }

    triggers {

        pollSCM '* * * * *'

    }

    stages {

        stage('Build') {

            steps {

                echo "Building.."

                sh '''
                mkdir folder

                '''

            }

        }

        stage('Test') {

            steps {

                echo "Testing.."

                sh '''

                cd myapp

                python3.11 hello.py
                docker ps


                '''

            }

        }

        stage('Deliver') {

            steps {

                echo 'Deliver....'

                sh '''

                echo "doing delivery stuff.."

                '''

            }

        }


    }

}
