@Library("belajar-jenkins-shared-library@main") _

// pznPipeline([
//     type: "maven"
// ])

import ambonxnobody.jenkins.Output;

pipeline {
    agent any

    stages {
        stage("Maven Compile") {
            steps {
                script {
                    maven(["clean", "compile", "test"])
                }
            }
        }
        
        stage("Global Variable") {
            steps {
                script {
                    echo(author())
                    echo(author.name())
                    echo(author.channel())
                }
            }
        }
        
        stage("Hello World") {
            steps {
                script {
                    hello.world()
                    hello.person([
                        firstName: "Hafid",
                        lastName: "Dian Nurfaujan Ahat"
                    ])
                }
            }
        }

        stage("Hello Ambon") {
            steps {
                script {
                    Output.hello(this, "Ambon")
                }
            }
        }
    }
}
