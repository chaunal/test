node
{
stage 'Clean'
    deleteDir()

    
stage 'a'
sh "echo 'hello stage a'"


def constants

stage('Import dependencies')
   git(url: 'https://github.com/chaunal/test', credentialsId: '19d257e9-5c61-4f50-a8fa-8d27ea76180a')
  constants = load('test.properties')
    
    println constants.getProperty('a')
}


