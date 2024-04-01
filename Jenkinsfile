pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                
         sh '''#!/bin/bash
                 mvn clean deploy sonar:sonar
                 
         '''
                
            }
        }
        stage('Test') {
            steps {
                 echo 'Test....'
            }
        }
        stage('Super test') {
            steps {
                 echo 'Super Test....'
            }
        }
    }
}
