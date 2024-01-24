pipeline{
agent none
  stages {
     stage ('A') {
       agent {label 'slave1'}
      steps {
        echo "this is a"
        
      }
    }
    stage ('run parallel b and t') {
      parallel { 
    stage ('B') {
      agent {label 'built-in'}
      steps {
        echo "this is b"
      }
    }
    stage ('T') {
      agent {label 'slave2'}
      steps {
        echo "this is t"
      }
    }
      }
    }
        stage ('run parallel d and e') {
      parallel {
    stage ('D') {
      agent {label 'lib1'}
      steps {
        echo "this is d"
        
      }
    }
        stage ('E') {
          agent {label 'slave2'}
      steps {
        echo "this is e"
        
      }
    }
      }
    }
  }
  
}
