pipeline {
	agent any
	stages{
		stage('Clean'){
			steps{
				withMaven(maven : 'Maven 3.6.0'){
				sh "mvn clean"
				}
			}
		}
		stage('test'){
			steps{
				withMaven(maven : 'Maven 3.6.0'){
				sh "mvn test"
				}
			}
		}
		stage('package'){
			steps{
				withMaven(maven : 'Maven 3.6.0'){
				sh "mvn package"
				}
			}
		}
	}
}
