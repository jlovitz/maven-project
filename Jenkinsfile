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
		sh  'docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}
