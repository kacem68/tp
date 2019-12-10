pipeline {
agent any
 tools {
  maven 'Maven 3.6.2'
 jdk jdk1.8.0_201
  
}
stage {
stage('build'){
steps{
bat 'mvn install'
}
post{
junit 'target/surefire-reports/**/*.xml'
}
}

}
}


}