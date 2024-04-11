## 1. Create the Personal Access Token

Developer Settings: Personal Access Tokens: Generate New Token: Note: (why you create this token ?) Select Scopes: (select repo)

## 2. Generate and Copy and Set Your Token
Check Current Remote URL, ensure your repository remote URL is set up to use HTTPS
```bash
git remote -v
```

YOU already cloned the project :
```bash
git remote set-url origin https://USERNAME:TOKEN@github.com/USER/REPOSITORY.git
```

YOU created the project locally (remote is not set or you're setting it up for the first time) :

```bash
git remote add origin https://USERNAME:TOKEN@github.com/USER/REPOSITORY.git
```

## 3. Stage and Commit Your Changes

```bash
git add .
git commit -m "Your commit message"
git push
```
(eventually git `push origin main` if project with branches)

