stage 'Compile'
node() {
    checkout scm
    // use for non multibranch: git 'https://github.com/amuniz/maven-helloworld.git'
    def mvnHome = tool 'apache-maven-3.6.0'
    sh "${mvnHome}/bin/mvn clean install -DskipTests"
    stash 'working-copy'
}
