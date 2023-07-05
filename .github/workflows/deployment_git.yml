
name : deployment_ex1
on : push
jobs :
 deploy :
    runs-on: windows-latest
    steps :
        - name : get the code
          uses : actions/checkout@v3
        - name : install NodeJS
          uses : actions/setup-node
          with :
            node-version : 18
        - name : install dependencies
          run : npm ci #or npm install
        #   running lint script and build script and output some deploy message
        - name : lint 
          run : npm run lint #to run lint script
        - name : test code
          run : npm run test 
        - name : build code
          run : npm run build #to run diff script from pacjage.js
        - name : deploy code
          run : echo "deploying as part of workflow.."
        



          
