pipeline
{
	agent any
	Stages
	{
		stage('Build')
		{steps{ sh 'mvn clean package'}}
	}
	post
	{
		success
		{archiveArtifacts artifacts:'target/*.jar', fingerprint:true}
	}
}
