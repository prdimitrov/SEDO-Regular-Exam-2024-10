node {  
    stage('Restore dependencies') { 
        bat 'dotnet restore'
    }
    stage('Build') { 
        bat 'dotnet build --no-restore'
    }
    stage('Test') { 
        bat 'dotnet test --no-build --verbosity normal'
    }
}
