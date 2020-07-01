node('master')
{
    stage('ContinuousDownload_Master') 
    {
      git 'https://github.com/vaishnavi972/Maven.git'
    }
    stage('ContinuousBuild_Master') 
    {
      sh label: '', script: 'mvn package'
    }
    stage('ContinuousDeployment_Master') 
    {
      sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/MultibranchPipeline_master/webapp/target/webapp.war ubuntu@172.31.30.28:/var/lib/tomcat8/webapps/testapp.war'
    }
}
