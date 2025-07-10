pipeline {
    agent { 
        node {
            label 'agentwithpython'
            }
      }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                cd myapp
                ls -ltr
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                python3 helloworld.py
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
