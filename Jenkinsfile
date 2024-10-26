node {
    stage('Restore dependencies') {
        dir('') {
            bat 'dotnet restore HouseRentingSystem.sln'
        }
    }
    stage('Build') {
        dir('') {
            bat 'dotnet build HouseRentingSystem.sln --no-restore'
        }
    }
    stage('Test') {
        dir('HouseRentingSystem.Tests') {  // Navigate to the test project directory
            bat 'dotnet test --no-build --verbosity normal'
        }
    }
}
