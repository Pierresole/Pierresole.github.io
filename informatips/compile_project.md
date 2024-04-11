Good practices, to install projects without any doubts

## 1. Cloning the Repository:

```bash
mkdir -p ~/projects
cd ~/projects
git clone https://github.com/username/project.git
```

Eventually create subfolders.

## 2. Building the Project:

For projects that require compilation (like C/C++ projects using Make or CMake), it's a good practice to create a separate build directory within the project folder.
Keep sources clear, for multiple build or cleanup 'rm -rf build'.

```bash
cd ~/projects/project
mkdir build && cd build
cmake ..  # Or any other build system command
make
```

## 3. Storing Build Artifacts:

The executable binaries or artifacts can be moved to `~/bin`
Don't forget to exclude build from version control by listing into `.gitignore`file.

Always prefer local or user-specific installation paths (e.g., `~/.local/bin`) for personal projects to avoid interfering with system-wide binaries.


## 4. Environment Variables:

If executables in non-standard directories : `~/projects/project/bin` or `~/.local/bin`, need to add to `PATH` environment

For projects that depend on specific libraries located outside standard system paths, you might need to adjust the `LD_LIBRARY_PATH` (Linux) environment variables. 


```bash
```

