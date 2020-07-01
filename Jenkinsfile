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
}
