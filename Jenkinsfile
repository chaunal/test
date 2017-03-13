node
{
stage 'Clean'
    deleteDir()

    
stage 'a'
sh "echo 'hello stage a'"


def constants

stage('Import dependencies')
  git(url: 'https://github.com/chuanal/test')
    constants = load('constants.groovy')
}
