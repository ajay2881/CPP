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
def jsonSlurper = new JsonSlurper()  
def jsonresp= '{ "name": "John", "ID" : "1"}'
def object = jsonSlurper.parseText(jsonresp)   
if (object.name=='John')
{
print 'hey name matched';
}
else
{ 
println 'name didnt match' 
} 
		
		}
	}

