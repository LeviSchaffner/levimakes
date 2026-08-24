# ./arcade

A small static game shelf for GitHub Pages.

## Publish with GitHub Pages

1. Create a GitHub repository and upload the contents of this folder.
2. In **Settings > Pages**, set **Source** to **Deploy from a branch**.
3. Select the branch containing `index.html` and the `/ (root)` folder.
4. Open the Pages URL GitHub provides.

The site uses relative paths, so it works from a repository Pages URL. Keep each game's web export and downloadable build inside its game folder.

## Add a game

Add a new object to the `games` array in `index.html` with `title`, `description`, `date`, `web`, and `windows` values. Copy the complete Godot web export into the referenced folder.

## Preview locally

```powershell
python -m http.server 8000
```

Open `http://localhost:8000` in a browser. Godot web exports need a web server and should not be opened directly from the filesystem.
