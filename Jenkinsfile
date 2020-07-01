node('master')
{
    stage('ContinuousDownload') 
    {
      git 'https://github.com/vaishnavi972/Maven.git'
    }
    stage('ContinuousBuild') 
    {
      sh label: '', script: 'mvn package'
    }
}
