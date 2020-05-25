pipeline
{
agent any
	stages{
		stage('build'){
			steps{
				cmd 'mvn -f Filecopy.parent/pom.xml clean install package'
				 }
					}
		stage('push'){
			steps{
				echo "hello"
				 }
					}
		stage('deploy'){
			steps{
				echo "hello"
				 }
					}
		}
}