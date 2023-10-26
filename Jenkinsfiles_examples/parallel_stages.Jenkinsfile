
node() {
  stage('test parallel stages') {
    def stages = [:]

    stages["s1"] = {
      echo "hello from stage 1"
    }

    stages["s2"] = {
      echo "hello from stage 2"
    }

    parallel(stages)
  }
}
