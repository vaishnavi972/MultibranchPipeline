node('master')
{
    stage('ContinuousDownload') 
    {
      git 'https://github.com/vaishnavi972/MultibranchPipeline.git'
    }
    stage('ContinuousBuild') 
    {
      sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment') 
    {
      sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/MultibranchPipeline_master/webapp/target/webapp.war ubuntu@172.31.30.28:/var/lib/tomcat8/webapps/testapp.war'
    }
}

