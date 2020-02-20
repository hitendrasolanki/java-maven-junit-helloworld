/******************************************************************
******Description :: This is Multibranch Pipeline Jenkinsfile******
******************************************************************/

node
  {
  /* checkout code from repo */
  stage('checkout')
    {
    checkout scm
    }
	/* Builds code based on branch name */
    stage('build')
    {
    echo 'branch name ' + env.BRANCH_NAME
    
    if (env.BRANCH_NAME.startsWith("Feature"))
      {
      echo "Building in feature Branch"
      }
      
    else if (env.BRANCH_NAME.startsWith("Develop"))
      {
      echo "Building in develop Branch"
      }
      
    else if (env.BRANCH_NAME.startsWith("master"))
      {
      echo "Building in master Branch"
      }
      
    /* sh """chmod +x HelloWorld.bat */
    /* ./HelloWorld.bat""" */
     
    echo "Hi! This is Multibranch Test-V1"
	    echo "Hi! This is Multibranch Test-V2"
 
    }
}
