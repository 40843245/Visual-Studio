# upgrade assistant tool in CLI
## migrate project
use `upgrade-assistant upgrade` command to migrate project.

### 1th way (Recommend) (used in offical tutorial) 

Step 1:

Open Visual Studio Command Prompt.

One way to do so is to select `tool` -> `command line` -> `command line prompt for developer`.

<img width="384" alt="image" src="https://github.com/user-attachments/assets/a932f4d2-55fe-4ed9-80c3-dbc2d5bdd7ea" />

Step 2:

Find the root directory of the project

Then copy it.

Step 3:

Change the current directory to root directory of the project.

To do so, 

In Visual Studio Command Prompt, use `cd` command.

```
cd <root-directory>
```

Step 4:

To migrate the project,

In Visual Studio Command Prompt, use `upgrade-assistant` command.

```
upgrade-assistant upgrade
```

#### reference
##### official website
[`upgrade assistant`](https://dotnet.microsoft.com/en-us/platform/upgrade-assistant)

### 2th way

Step 1:

Open Visual Studio Command Prompt.

One way to do so is to select `tool` -> `command line` -> `command line prompt for developer`.

<img width="384" alt="image" src="https://github.com/user-attachments/assets/a932f4d2-55fe-4ed9-80c3-dbc2d5bdd7ea" />

Step 2:

Find the root directory of the project

Then copy it.

Step 3:

To migrate the project,

In Visual Studio Command Prompt, use `upgrade-assistant` command.

```
upgrade-assistant upgrade <root-directory>
```
