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
	 
	stage('OS_TYPE_JOB_BASE_NAME ') {
            steps {
                sh ''' echo ${JOB_BASE_NAME} '''
            }	
        } 
	    
	    
	stage('run sh ') {
            steps {
		sh "chmod +x -R ${env.WORKSPACE}"
                sh ''' ./test.sh '''
            }	
        } 
	  
	JOB_BASE_NAME
	    
    }
}
