# How deploy Storybook to Github Pages

1. Create React App

```bash
npx create-react-app my-app
```

2. Run your React App

```bash
npm start
```

3. Init storybook

```bash
npx storybook init
```

4. Run storybook

```bash
npm run storybook
```

5. Edit build-storybook script in package.json

```json
{
  "build-storybook": "build-storybook -o docs -s ./src/stories/assets",
}
```

6. Add homepage in package.json

```json
{
  "homepage": "https://NAME_ACCOUNT.github.io/REPOSITORY_NAME"
}
```

7. Add ssh url

```bash
git remote add origin REPOSITORY_URL
```

8. Add files to commit

```bash
git add .
```

9. Commit changes

```bash
git commit -m "init"
```

10. Push changes

```bash
git push origin master
```

11. Set `/docs` source in `Repository/Settings/Pages/Source`

12. Check your React App in https://NAME_ACCOUNT.github.io/REPOSITORY_NAME
