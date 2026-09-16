//GPE104 — Project 1, Milestone 2: Source Control Setup

//Student: Christian Mederos
//Course: GPE104 — Game Programming
//Unity Version:6000.6.0f1 
//Repository:[https://github.com/CMederos13/gpe104-project1-2] (https://github.com/CMederos13/gpe104-project1-2)
//Youtube: [https://youtu.be/x11143wz8xY] (https://youtu.be/x11143wz8xY)
** Overview **

This milestone connects a Unity project to a public GitHub repository using Git for source control, and demonstrates a full branch > change > merge workflow.

// 1. Public GitHub repository

A public repository was created at [github.com/CMederos13/gpe104-project1-2](https://github.com/CMederos13/gpe104-project1-2). Public visibility was chosen specifically so the repo can be reviewed without needing a collaborator invite.

// 2. Unity project connected and pushed

A new Unity project was created locally, initialized as a Git repository with `git init`, connected to the GitHub repo with `git remote add origin`, and pushed with `git push -u origin main`. The project includes a `Scripts` folder under `Assets` and a main scene named `Main` (`Assets/Scenes/Main.unity`), 

// 3. `.gitignore`

A Unity-appropriate `.gitignore` was added at the project root (same level as the `Assets` folder), excluding generated/local folders and files such as `Library/`, `Temp/`, `Obj/`, `Build/`, `Builds/`, `Logs/`, `UserSettings/`, `.vs/`, `.idea/`, `*.csproj`, `*.sln`, and `*.userprefs`. This keeps the repository free of Unity's regenerated cache files

// 4. Branching workflow

A branch:

- A new branch named `dev` was created off `main` with `git branch -c dev` and switched to with `git switch dev`.
- Changes were made on `dev`: a `HelloWorld.cs` script was added to `Assets/Scripts`, later edited to include a `Debug.Log("Hello, World!")` call in `Start()`, and finally removed as a cleanup step — each change committed separately with a descriptive message.
- `dev` was pushed to GitHub with `git push -u origin dev`.
- The branch was merged back into `main` with `git switch main` followed by `git merge dev`.(no conflicts, since `main` had not changed independently while `dev` was being worked on).
- The merged `main` was pushed back to GitHub with `git push`.

//5. Commit history

All commits with be in the commits section
