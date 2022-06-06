# How deploy React App to Github Pages

> For Github Pages use `react-router-dom/HashRouter` instead `react-router-dom/BrowserRouter`

---

1. Create React App

```bash
npx create-react-app my-app
```

2. Run your React App

```bash
npm start
```

3. Add ssh url

```bash
git remote add origin REPOSITORY_URL
```

4. Install package for github pages

```bash
npm install gh-pages --dev
```

5. Add deploy script in package.json

```json
{
  "deploy": "npm run build && gh-pages -d build"
}
```

6. Add homepage in package.json

```json
{
  "homepage": "https://NAME_ACCOUNT.github.io/REPOSITORY_NAME"
}
```

7. Add files to commit

```bash
git add .
```

8. Commit changes

```bash
git commit -m "init"
```

9. Push changes

```bash
git push origin master
```

10. Deploy your React App to Github Pages

```bash
npm run deploy
```

11. Check your React App in https://NAME_ACCOUNT.github.io/REPOSITORY_NAME
