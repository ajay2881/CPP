#!groovy
import groovy.json.JsonSlurper
node {
	stage('Example') {
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
    }
