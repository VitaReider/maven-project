pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven: 'maven_3_5_0') {
                    // Run the maven build
                    bat "mvn clean compile"
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven: 'maven_3_5_0') {
                    // Run the maven test
                    bat 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(maven: 'maven_3_5_0') {
                    // Run the maven deployment
                    bat 'mvn deploy'
                }
            }
        }
    }
}