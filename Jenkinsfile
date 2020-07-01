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
}
