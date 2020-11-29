pipeline {
        agent none        
        tools {
                maven 'my_mvn'
        }
        stages {
            stage ("Compile") {
                    agent {
                            label "Slave_Node_1"
                        }
                steps {
                        sh "mvn compile"
                    }
                }        
            stage("unit test") {  
                    agent {
                            label "Slave_Node_2"
                        }
                    steps {
                        sh "mvn test"
                    }
            }
        }
}
