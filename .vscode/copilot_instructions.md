# GitHub Copilot Instructions for Wingman Project

## Launch & Task Settings

This project has established VS Code configurations for running and debugging:

1. **Use existing task configurations**

   - Always prefer using the `run_vs_code_task` tool with the tasks defined in `.vscode/tasks.json`
   - Available tasks:
     - `Flutter: Run` - Builds and runs the app on Windows
     - `Flutter: Hot Reload` - For hot reloading code changes
     - `Flutter: Hot Restart` - For hot restarting the app

2. **Launch Settings**

   - Use the launch configuration in `.vscode/launch.json`
   - Debug configuration name: "Flutter: Wingman"

3. **Never use direct shell commands for Flutter**

   - Do not use `flutter run`, `flutter build`, etc. directly via terminal
   - Always use VS Code tasks instead

4. **Hot Reload Notes**
   - Hot reload is supported for most changes
   - State is preserved during hot reload
   - App does not need to be fully restarted for UI changes

## Build Preferences

- Target platform: Windows
- Build in debug mode during development
- Always validate code before building

## Project Specific Notes

- This is a Flutter desktop application (not web or mobile)
- Uses Riverpod for state management
- UI follows Material 3 design principles
- All file operations should use proper error handling
