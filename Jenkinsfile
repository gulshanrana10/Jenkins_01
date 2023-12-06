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


                '''

            }

        }

        stage('Test') {

            steps {

                echo "Testing.."

                sh '''

                cd myapp

                python3.11 hello.py


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
         stage('Saksi') {

            steps {

                echo 'Goodnight....'

                sh '''

                echo "you should sleep.."

                '''

            }

        }

    }

}
