node("docker") {
    stage('Checkout') {
        checkout scm
    }

    stage('dump env') {
        env.each { name, value -> println "Name: $name -> Value $value" }
    }
}
