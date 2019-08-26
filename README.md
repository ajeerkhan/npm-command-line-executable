# npm-command-line-executable
How to make npm package as command-line executable

# Make / register js script file as executable in your computer.

Step #1. Create a nodejs project.
      run "npm init" within your project folder.
Step #2. Create a script file in project, mentioning below script at top.
          #!/usr/bin/env node
        above indidate that "node" is the interpreter for this script file.
      
Step #3. add "bin" entry in package.json, passing command-name and corresponding executable script file.

            "bin": {
                    "sayhello": "./script.js"
                },
    
Step #4. Create Links globally in npm package

    run "npm link" in your project folder, which create a link globally under roaming/npm/

Thats all!!! here we go with testing the CLI created!!!.

# verification
run "sayhello" in your command prompt, which would show "Hello world!". 

Congratulation!!! you have successfully learned new things!!!!

Note: when you refer the node module with "command executable" defined in your project , and run "npm install", npm symlink named executable commands as 

    ./node_modules/.bin/ for local installs
     prefix/bin for global modules


