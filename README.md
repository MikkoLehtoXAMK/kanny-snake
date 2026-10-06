# Känny Snake: your first Git project

This is a tiny snake game. You'll use it to learn the one Git skill you'll need first: **working on the same project in two places** without losing anything.

Think of Git as a save system for your work.

| Git word | What it means in game terms |
|---|---|
| Commit | Make a save point, with a note about what changed |
| Push | Upload your saves to the cloud (GitHub) |
| Pull | Download the newest saves from the cloud |
| Discard | Reload your last save |

In this exercise, the **GitHub website** plays your "school computer" and **GitHub Desktop** on your own machine is "home".

---

## Before you start

You need a GitHub account and GitHub Desktop installed and signed in. If you did the pre-task, you're ready.

**Mac users:** don't edit files in TextEdit. It swaps normal quote marks `"` for curly ones `“ ”` and the game breaks. Either do your edits on the GitHub website, or install [VS Code](https://code.visualstudio.com/) (free) and edit there.

---

## 1. Make your own copy

1. At the top of this page, click the green **Use this template** button, then **Create a new repository**.
2. Give it a name, like `my-snake`. Private is fine.
3. Click **Create repository**.

You now have your own copy on GitHub. It's yours. You can't break anyone else's.

## 2. Download it to your computer (clone)

1. On **your** new repository page, click the green **Code** button.
2. Click **Open with GitHub Desktop**.
3. GitHub Desktop opens. Click **Clone**.

"Clone" just means: download it, and keep it connected to GitHub.

## 3. Play it

1. In GitHub Desktop, go to **Repository > Show in Explorer** (on a Mac: **Show in Finder**).
2. Double-click `index.html`. The game opens in your browser.
3. Press **5** or **space** to start. Steer with the arrow keys.

## 4. Change something, then save it to the cloud

1. Open `settings.js`. On Windows: right-click it, **Open with > Notepad**.
2. Change one value. For example, make `SNAKE_SPEED` 9, or `SCREEN_THEME` "pink".
3. Save the file. Refresh the game in your browser. Your change is there.
4. Look at GitHub Desktop. It shows exactly what you changed: red is the old line, green is the new one.
5. Bottom left, type a short note in **Summary**, like `Faster snake`.
6. Click **Commit to main**. That's your save point.
7. Click **Push origin** at the top. Your save is now in the cloud.

Do this two or three times with different settings. Commit after each change.

## 5. Work on the "school computer"

Pretend you're at school now, on a computer that isn't yours.

1. Go to your repository on the GitHub website.
2. Click `settings.js`, then the **pencil icon** (Edit this file).
3. Change a different value. Maybe your `GAME_TITLE`.
4. Click **Commit changes**, then **Commit changes** again in the pop-up.

Now GitHub has a change that your home computer doesn't have yet.

## 6. Back home: get the latest version (pull)

1. In GitHub Desktop, click **Fetch origin**. This checks the cloud for new saves.
2. The button changes to **Pull origin**. Click it.
3. Refresh the game in your browser. The change you made "at school" is there.

## 7. Break it on purpose, then fix it

1. Open `settings.js` and delete one of the `"` quote marks. Save.
2. Refresh the game. It says **CHECK SETTINGS.JS**. You broke it.
3. In GitHub Desktop, right-click `settings.js` in the Changes list and choose **Discard changes**.
4. Refresh the game. Fixed. You just reloaded your last save.

---

## The one rule to remember

**Pull when you sit down. Push when you get up.**

Start every work session by pulling. End every work session by committing and pushing. If you forget, the two places get out of sync, and fixing that is annoying. Your teacher will show you what it looks like.

---

## What else can I change?

Everything in `settings.js`:

- `GAME_TITLE`: the name on the start screen
- `SNAKE_SPEED`: 1 to 10
- `START_LENGTH`: 2 to 20
- `FOOD_POINTS`: points per food
- `WALLS_KILL`: `true` or `false`
- `SCREEN_THEME`: "green", "blue", "amber", "grey" or "pink"
- `PHONE_COLOUR`: a colour name like "tomato" or a hex code like "#2e8b57"
- `SOUND_ON`: `true` or `false`
- `GAME_OVER_TEXT`: what the screen says when you lose

Leave `index.html` alone unless you know what you're doing. Or don't. You can always discard your changes.
