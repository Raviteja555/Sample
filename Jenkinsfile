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
				cd C:\Program Files (x86)\Jenkins\workspace\filecopypipeline\Filecopy\target
				docker build -t target\Filecopy_1.0.0.ear .
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
