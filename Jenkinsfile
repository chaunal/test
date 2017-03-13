node
{
stage 'Clean'
    deleteDir()

    
stage 'a'
sh "echo 'hello stage a'"


def constants

stage('Import dependencies')
  git(url: 'https://github.com/chuanal/test', credentialsId: '19d257e9-5c61-4f50-a8fa-8d27ea76180a')
    
	Properties props = new Properties()
	File propsFile = new File('test.properties')
	props.load(propsFile.newDataInputStream())
	println props.getProperty('a')
}
