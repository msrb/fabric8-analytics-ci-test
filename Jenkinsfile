node("docker") {
    stage('Checkout') {
        checkout scm
    }

    stage('dump env') {
        sh 'env > env.txt'
        readFile('env.txt').split("\r?\n").each {
            println it
        }
    }
}
