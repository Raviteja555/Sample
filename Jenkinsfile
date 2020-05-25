pipeline
{
agent any
	environment{

	DOCKERPASS=credential(dockercred)
	}
	stages{
		stage('build'){
			steps{
				bat '''
				mvn -f Filecopy.parent/pom.xml clean install package
				echo $DOCKERPASS
				'''
			
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