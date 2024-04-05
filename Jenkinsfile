@Library("belajar-jenkins-shared-library@main") _

// pznPipeline([
//     type: "maven"
// ])

import ambonxnobody.jenkins.Output;

pipeline {
    agent any

    stages {
        stage("Hello World") {
            steps {
                script {
                    hello.world()
                }
            }
        }

        stage("Hello Ambon") {
            steps {
                script {
                    Output.hello("Ambon")
                }
            }
        }
    }
}
