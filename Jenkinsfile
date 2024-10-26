node {
    stage('Restore dependencies') {
        dir('HouseRentingSystem.Tests') {  
            bat 'dotnet restore'
        }
    }
    stage('Build') {
        dir('HouseRentingSystem.Tests') {
            bat 'dotnet build --no-restore'
        }
    }
    stage('Test') {
        dir('HouseRentingSystem.Tests') {
            bat 'dotnet test --no-build --verbosity normal'
        }
    }
}
