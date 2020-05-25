pipeline
{
agent any
	environment{

	DOCKERPASS = credentials('dockercred')
	}
	stages{
		stage('build'){
			steps{
				bat '''
				mvn -f Filecopy.parent/pom.xml clean install package
				echo  %DOCKERPASS_USR%  %DOCKERPASS_PSW%
				'''
			
				 }
					}
		stage('push'){
			steps{
				bat 'echo %DOCKERPASS_USR%'
				 }
					}
		stage('deploy'){
			steps{
				echo "hello"
				 }
					}
		}
}