pipeline {
  agent any
    stages {

      stage('Build Blender') {
        when {
          changeset "blender/**"
        }
        steps {
          sh 'kiss-ci blender'
        }
      }

      stage('Build CMake') {
        when {
          changeset "cmake/**"
        }
        steps {
          sh 'kiss-ci cmake'
        }
      }

      stage('Build Firefox') {
        when {
          changeset "firefox/**"
        }
        steps {
          sh 'kiss-ci firefox'
        }
      }

      stage('Build GCC') {
        when {
          changeset "gcc/**"
        }
        steps {
          sh 'kiss-ci gcc'
        }
      }

      stage('Build LLVM') {
        when {
          changeset "llvm/**"
        }
        steps {
          sh 'kiss-ci llvm'
        }
      }

      stage('Build Node.js') {
        when {
          changeset "nodejs/**"
        }
        steps {
          sh 'kiss-ci nodejs'
        }
      }

      stage('Build Rust') {
        when {
          changeset "rust/**"
        }
        steps {
          sh 'kiss-ci rust'
        }
      }

    }
}
