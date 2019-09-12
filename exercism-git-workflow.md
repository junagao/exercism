# Exercism Git Workflow

1. On the new exercise folder initialize git

   ```bash
   git init
   ```

2. Set remote url to new repository

   ```bash
   git remote add origin git@github.com:junagao/darts.git   
   ```

3. Create .gitignore

   ```json
   /.exercism
   /node_modules
   ```

4. Add all initial files and commit it

   ```bash
   git add .
   git commit -m 'initial commit'
   git push
   ```

5. Install dependencies

   ```bash
   npm i
   ```

6. Add package and commit

   ```bash
   git add .
   git commit -m 'feat: install dependencies'
   ```

7. Add solution and commit it

   ```bash
   git add .
   git commit -m 'feat: add darts solution'
   ```

8. Go to exercism/javascript and add submodule to exercism repo:

   ```bash
   git submodule add git@github.com:junagao/darts.git darts
   git commit -m "feat: add darts submodule"
   ```



Notes:

<https://github.blog/2016-02-01-working-with-submodules/>