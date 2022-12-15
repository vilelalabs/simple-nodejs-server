pipeline{
    agent any

    stages{
        stage('Build Image'){
            steps{
                script{
                    dockerapp = docker.build("simplenodeserver:latest", "-f ./src/Dockerfile ./src")
                }
                echo 'Building'
            }
        }
    }


    // stages{
    //     stage('Build'){
    //         steps{
    //             echo 'Building'
    //         }
    //     }
    //     stage('Test'){
    //         steps{
    //             echo 'Testing'
    //         }
    //     }
    //     stage('Deploy'){
    //         steps{
    //             echo 'Deploying'
    //         }
    //     }
    }
}