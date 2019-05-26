stage 'Compile'
node('linux1') {
    checkout scm
    // use for non multibranch: git 'https://github.com/amuniz/maven-helloworld.git'
    def mvnHome = tool 'maven-3'
    sh "${mvnHome}/bin/mvn clean install -DskipTests"
    stash 'working-copy'
}
