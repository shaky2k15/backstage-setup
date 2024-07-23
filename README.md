# backstage-setup
setup steps
1. NVM Upgrade in macos using following link https://dev.to/mkubdev/how-to-install-nvm-on-macos-with-homebrew-gfn
2. Upgrade vscode in mac using homebrew command "brew upgrade visual-studio-code"
3. docker , git , yarn should have been installed already in mac
4. Follow the steps for backstage setup
During setup this error may be encountered
"Error: @backstage/create-app requires Yarn v1, found '3.8.1'. You can migrate the project to Yarn 3 after creation using https://backstage.io/docs/tutorials/yarn-migration
It seems that something went wrong when creating the app 🤔
🔥  Failed to create app!"

Fix for this -> "yarn set version 1.22.19"
https://stackoverflow.com/questions/76513866/issue-creating-the-backstage-app-using-npx-backstage-create-app

5. During the local startup of backstage instance , while creating a task following error may be encountered 
"When using Node.js version 20 or newer, the scaffolder backend plugin requires that it be started with the --no-node-snapshot option.  Please make sure that you have NODE_OPTIONS=--no-node-snapshot in your environment."
Fix for this -> "export NODE_OPTIONS=--no-node-snapshot" in the terminal window before running yarn dev command

6. Once app is created, go to the app folder and create a plugin.
7. To create app follow this page https://backstage.io/docs/getting-started/
8. To create plugin follow this page https://backstage.io/docs/plugins/create-a-plugin
9. localhost:3000 will be app page , localhost:3000/my-plugin will be plugin page (here my-plugin is the name/label of example plugin)
10. Following versions are working properly for me
npm -v 10.7.0
node -v v20.15.0
yarn -v 1.22.19
nvm -v 0.39.7
