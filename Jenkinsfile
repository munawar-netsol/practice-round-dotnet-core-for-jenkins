pipeline {
    agent any
	stages
	{            
		stage('Four') {
			parallel {
				stage('Unit Testing') {
					steps {
						sh 'dotnet build TeacherService/TeacherService.csproj'
						sh 'dotnet build StudentService/StudentService.csproj'
					}
					
				}
			}
		}
	}
}