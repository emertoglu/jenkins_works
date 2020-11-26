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
                sudo sh('../test/test.sh')
            }	
        }
    }
}
