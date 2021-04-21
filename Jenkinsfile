#!groovy
import groovy.json.JsonSlurperClassic
node {
  
    def BRANCH_NAME = env.BRANCH_NAME    
   
	    stage('checkout source') {
        		// when running in multi-branch job, one must issue this command
        		checkout scm
	    }      
 	
       		if (env.BRANCH_NAME == "Dev")  {
			print "hi from dev branch"
		
		}
	}

