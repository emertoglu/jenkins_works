pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                echo 'jenkins github testing'
            }
        }
		stage('build') {
            steps {
                sh('../test/test.sh')
            }	
        }
    }
}
