	pipeline {
    agent any

    stages {
        stage('Prod Deploy') {
            when {
                branch 'master'
            }
            steps {
                
                input message: 'Are you sure you want to deploy to prod (Click "Proceed" to continue)'
				echo 'Prod deployed'
                
            }
        }
        stage('Dev Deploy') {
            when {
                branch 'dev'
            }
            steps {
               
				echo 'Dev deployed'
            }
        }
		
		 stage('UAT Deploy') {
            when {
                branch 'uat'
            }
            steps {
                input message: 'Are you sure you want to deploy to UAT (Click "Proceed" to continue)'
				echo 'UAT deployed'
            }
        }
    }
}
