node {
   stage('Preparation') {
      git 'https://github.com/ashukatayev/SimpleWebAppHeroku.git'
   }
   stage('Build') {
      sh "./gradlew clean test"
   }
   stage('Deploy') {
   sh "git push https://git.heroku.com/sleepy-anchorage-80491.git master"
   }
}