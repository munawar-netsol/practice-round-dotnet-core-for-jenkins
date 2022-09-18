pipeline {
    agent any
	stages
	{            
		stage('Four') {
			parallel {
				stage('Code Build') {
					steps {
						sh 'dotnet build TeacherService/TeacherService.csproj'
						sh 'dotnet build StudentService/StudentService.csproj'
					}
					
				}
			}
		}
	}
}