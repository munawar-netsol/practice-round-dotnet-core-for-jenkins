pipeline {
    agent any
	stages
	{            
		stage('Four') {
			parallel {
				stage('Unit Testing') {
					steps {
						sh 'dotnet build TeacherService/TeacherService.csproj'
					}
					
					steps {
						sh 'dotnet build TeacherService/StudentService.csproj'
					}
				}
			}
		}
	}
}