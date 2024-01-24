pipeline{
agent any
  stages {
     stage ('A') {
      steps {
        echo "this is a"
      }
    }
    stage ('run parallel b and t') {
      parallel { 
    stage ('B') {
      steps {
        echo "this is b"
      }
    }
    stage ('T') {
      steps {
        echo "this is t"
      }
    }
      }
    }
        stage ('run parallel d and e') {
      parallel {
    stage ('D') {
      steps {
        echo "this is d"
        
      }
    }
        stage ('E') {
      steps {
        echo "this is e"
        
      }
    }
      }
    }
  }
  
}
