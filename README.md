name: CI

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [  ]

jobs:atest

  build:

   

    steps:
    - uses: actions/checkout@v4
    - name: Use Node.js
      uses: actions/setup-node@v4
      with:
        node-version: ''

   
    
    - run: npm install


