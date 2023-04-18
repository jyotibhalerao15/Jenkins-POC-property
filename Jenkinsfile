
pipeline {
    agent any
    stages {
        stage ("Test Stage"){
            steps {
                script {
                    def props = readProperties  file:'./test.properties'
                    def Var1= props['Monday']
                    def Var2= props['Tuesday']
                    echo "Var1=${Var1}"
                    echo "Var2=${Var2}"
                    echo "Inside stage1"
                }
            }
        }
        stage("Test Stage2"){
            steps{
                echo "Inside Stage 2"
                echo "Var1=${Var1}"
                echo "Var2=${Var2}"
            }
        }
    }
}
