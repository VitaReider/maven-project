pipeline {
    agent any
    stages{
        stage('Compile Stage'){
		
			steps {
				withMaven(maven : 'Apache Maven 3.5.2') {
					sh 'mvn clean compile'
				}
			}
		}
		
		stage('Deployment Stage'){
		
			steps {
				withMaven(maven : 'Apache Maven 3.5.2') {
					sh 'mvn deploy'
				}
			}
		}
    }
}