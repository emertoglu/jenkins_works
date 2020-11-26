pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                echo 'jenkins github testing'
            }
        }
	stage('WORKSPACE path') {
            steps {
                sh ''' echo ${WORKSPACE} '''
            }	
        }
	    
	stage('JENKINS_HOME path') {
            steps {
                sh ''' echo ${JENKINS_HOME} '''
            }	
        }    
	 
	stage('run sh ') {
            steps {
                sh ''' ./test.sh '''
            }	
        } 
	    
	    
    }
}
