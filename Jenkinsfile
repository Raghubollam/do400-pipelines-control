node('nodejs') {

 stage('Checkout') {

 git branch: 'main',

 url: 'https://github.com/Raghubollam/do400-pipelines-control'

 }

pipeline {

 agent {

 node {

 label 'nodejs'

 }

 }

stages {

 stage('Backend Tests') {

 steps {

 sh 'node ./backend/test.js'

 }

 }

 stage('Frontend Tests') {

 steps {

 sh 'node ./frontend/test.js'

 }

 }

 }

}

