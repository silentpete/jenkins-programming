node() {
  stage('test parallel commands') {
    parallel([
      c1: {
        echo "hello from c1"
      },
      c2: {
        echo "hello from c2"
      }
    ])
  }
}
