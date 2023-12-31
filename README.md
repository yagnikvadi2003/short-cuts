# short-cuts

## custom port
    yarn start --port 2003

## check packages(major, minor, patch)
    yarn outdated

## all packages upgrade
    yarn upgrade --latest

## Full information on your domain
    curl -I http://example.com

## Show free and used memory on your PC 
    free -m

## Create a new folder
    mkdir [folder name]

## Copy then paste your file
    cp [filename] [new filename] || cp [filename] [path/to/new/location/filename]

## present working directory
    pwd

## Print subdirectories of a directory
    ls -R

## shows the list of commands (with numeric numbers)
    history

## change password using terminal
    passwd

## prints a file’s last ten lines
    tail filename

## displays running processes and the system’s resource usage
    top

## show graph 
    git log --graph

## Git Diff to Compare Files
    git diff

# OR set an application state with name --name or -n
    pm2 start web.js --name "node-app-backend"
    
# Stop Process
    pm2 stop node-app-backend

# Restart Process
    pm2 restart node-app-backend

# Update Environment Variable
    NODE_ENV=production pm2 restart node-app-backend --update-env

# Delete Process
    pm2 delete node-app-backend

# List Processes
    pm2 list
# Or
    pm2 [list|ls|l|status]

# Reset Restart Count - this will reset the restart count
    pm2 reset all
# Sort Processes
    pm2 list --sort name:desc
# OR
    pm2 list --sort [name|id|pid|memory|cpu|status|uptime][:asc|desc]

# By default sorting field is name and the sorting order is asc
# Watch and Restart the app when files change
    pm2 start server.js --watch

# Delay between automatic restart of application
    pm2 start server.js --restart-delay <delay in ms>

# Do not auto restart application
    pm2 start server.js --no-autorestart

# MAX MEMORY RESTART
# PM2 allows to restart application based on memory limit
    pm2 start server.js --max-memory-restart 50M


