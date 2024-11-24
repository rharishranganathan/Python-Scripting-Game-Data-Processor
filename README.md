# Python-Scripting-Game-Data-Processor

This project is focused on creating a Python script to enhance Python scripting skills.The script automates the organization, compilation, and execution of game-related files in a specified data directory.

## Project Overview

This script is intended to work with a directory containing multiple game folders, each with a `.go` file. It performs the following tasks:
1. **Locate Game Directories**: Searches the source data folder for directories that contain the word "game."
2. **Create Target Directory**: Sets up a `/games` directory if it doesn't already exist.
3. **Copy and Rename Game Directories**: Transfers game directories to `/games`, removing the "game" suffix from each name.
4. **Generate JSON Metadata**: Creates a `metadata.json` file in `/games`, summarizing information about the games.
5. **Compile and Run Game Code**: Compiles each `.go` file in the game directories and runs the compiled code.

## Assumptions

- The **data directory** contains various files and folders.
- Only directories containing **"game"** in their name are relevant.
- Each **game directory** includes a single `.go` file that must be compiled and then executed.

## Files

- **get_game_data.py**: The main script implementing the steps listed above.

## Usage

To run the script, use the following command:

```bash
python get_game_data.py <source_directory> <target_directory>
