pipeline{
agent any
  stages {
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
    stage ('D') {
      steps {
        echo "this is d"
        
      }
    }
    
  }
  
}
