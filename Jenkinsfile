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
	    
	    
	 stage('environmentS  ') {
            steps {
                sh ''' echo ${BUILD_ID}''' 

		sh ''' echo ${BUILD_NUMBER} '''

		sh ''' echo ${BUILD_TAG} '''

		sh ''' echo ${BUILD_URL} '''

		sh ''' echo ${EXECUTOR_NUMBER} '''

		sh ''' echo ${JAVA_HOME} '''

		sh ''' echo ${JENKINS_URL} '''

		sh ''' echo ${JOB_NAME} '''

		sh ''' echo ${NODE_NAME} '''

		    sh ''' echo ${WORKSPACE} '''
            }	
        }    
	    
	stage('run sh ') {
            steps {
		sh "chmod +x -R ${env.WORKSPACE}"
                sh ''' ./test.sh '''
            }	
        } 
	  	
	    
    }
}
