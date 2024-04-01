pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                
         sh '''#!/bin/bash
                 mvn clean verify sonar:sonar \
  -Dsonar.projectKey=tester \
  -Dsonar.projectName='tester' \
  -Dsonar.host.url=http://localhost:55000 \
  -Dsonar.token=sqp_aa6ee1b8d413cb95def41b9f75d67b1f3a630767
                 
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
