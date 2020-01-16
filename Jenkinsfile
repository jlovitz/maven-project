pipeline {
    agent any

    tools {
        maven 'localMaven'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh  'mvn clean package'
            }
        }
    }
}
