ipeline{
    agent{label "build_server"}
        stages{
            stage("This stage will build package"){

                steps{
                    sh "mvn clean"
                    sh "mvn install"

            }
        }

        stage("This stage will copy the packages to the S3 bucket"){

                steps{ sh "aws s3 cp /home/ubuntu/build_server/workspace/declarative_pipeline_example/target/hello-world-project.war s3://mys3-10062023"

            }
        }
 }

}
