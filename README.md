# Upskillie-Open contribution guidelines
Guidelines people can follow while contributing to Upskillie open source projects.

## Code Structure

### Preferred Code Editor
- [Visual Studio Code](https://code.visualstudio.com/Download)

### Code Formatting Practices :
#### 1. Indentation
- Use `TAB` size `4` in indentation settings

#### 2. Styling
- Don't declare same css __class__ names at multiple places, if they are not supposed to be used there.
> For eg: If there is a component, you need to copy and modify, you need to change the classnames too to avoid the collisions

- Never use inline styling.
 
#### 3. Localization
- Static texts should be saved in their `locale` file
> For eg. English texts should be saved as `localization/en.js`

## How to use Git?
Common practices, you should follow while using git in your peojects

### Branching

#### Common Branches
There will be two common branches - `master` & `dev`

##### About `master` branch
 1.  This branch will only contain production code
 2.  Everyone should `checkout` from __master__ branch to create a `feature` or a `bugfix` branch
 3.  Steps involved:
    
    ```
      git checkout master 
      // Checking out to master branch

      git pull origin master 
      //Get the latest changes of master to your local system

      git checkout -b feature/feature-name 
      // Create and checkout to a new branch to implement your feature.

      or

      git checkout -b hotfix/bug-name
      // Create and checkout to a new branch to patch your bugfix logic.
      ```

##### About `dev` branch
1.  This branch will have all development code from all feature branches.
2.  Everyone should test their changes by pushing the code in dev branch first.
