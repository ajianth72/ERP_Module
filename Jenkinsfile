pipeline {
    agent any
    parameters {
        string(name:'Project Name',defaultValue:'Python_Project','description':'Enter Project Name')
        choice(name: 'Environment Name', choices: ['Dev', 'UAT', 'Prod'], description: 'Select Environment Name')
    }
    stages{
        stage('Build'){
            steps{
                echo "Im building Project from Git "
                echo "Build Number - ${env.BUILD_NUMBER}, Branch Name - ${env.BRANCH_NAME}, JOB_URL - ${env.JOB_URL}"
            }
        }
        stage('Test'){
            steps{
                echo "I'm in testing face"
            }
        }
        stage('Deploy'){
            steps{
                echo "I'm now in deployment stage"
            }
        }
    }
}
