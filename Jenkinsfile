pipeline {
    agent any
    stages {
        stage('Build Master') {
			when{
				branch 'master'
			}
			steps {                
				echo 'Building master'
			}
        }
		stage('Build Dev') {
			when{
				branch 'dev'
			}
			steps {                
				echo 'Building dev'
			}
        }
		stage('Build tags') {
			when{
				buildingTag()
			}
			steps {                
				echo 'Hello world Building tags'
			}
        }
    }
}
