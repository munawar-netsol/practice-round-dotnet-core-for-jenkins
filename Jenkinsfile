pipeline {
	agent {
		stages {
			stage('Build') {
				steps {
					sh 'dotnet build TeacherService/TeacherService.csproj'
				}
			}
		}
	}
}