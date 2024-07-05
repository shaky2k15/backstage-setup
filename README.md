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
