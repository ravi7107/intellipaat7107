pipeline{
    agent{label "build_server"}
        stages{
            stage("This stage will build package"){

                steps{
                    sh "mvn clean"
                    sh "mvn install"

            }
        }

    
 }

}
