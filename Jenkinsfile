pipeline {
	agent any
	stages{
		stage('Clean'){
			steps{
				withMaven(maven : 'Maven 3.6.0'){
				bat "mvn clean"
				}
			}
		}
		stage('test'){
			steps{
				withMaven(maven : 'Maven 3.6.0'){
				bat "mvn test"
				}
			}
		}
		stage('package'){
			steps{
				withMaven(maven : 'Maven 3.6.0'){
				bat "mvn package"
				}
			}
		}
	}
}
