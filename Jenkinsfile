@NonCPS
def printParams() {
  env.getEnvironment().each { name, value -> println "Name: $name -> Value $value" }
}

node("docker") {
    stage('Checkout') {
        checkout scm
    }

    stage('dump env') {
        printParams()
    }
}
