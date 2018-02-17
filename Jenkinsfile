pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                // Run the maven build
                bat "mvn clean compile"
            }
        }

        stage ('Testing Stage') {

            steps {
                // Run the maven test
                bat 'mvn test'
            }
        }

        stage ('Deployment Stage') {
            steps {
                // Run the maven deployment
                bat 'mvn deploy'
            }
        }
    }
}