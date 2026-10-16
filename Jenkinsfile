pipeline{
    agent any
///This is a simple Jenkins pipeline for a .NET project. It includes stages for restoring dependencies, building the project, and running tests. The 'bat' command is used to execute .NET CLI commands on Windows agents.
    stages{
        stage("Restore the project"){
            steps{
                bat "dotnet restore"
            }
        }
        stage("Build the project"){
            steps{
                bat "dotnet build"
            }
        }
        stage("Run the tests"){
            steps{
                bat "dotnet test --no-build --verbosity normal"
            }
        }
    }
}