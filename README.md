# CommonUser - Unreal Engine Plugin

This is the **CommonUser** plugin extracted from Epic Games' **Lyra Sample Game**, providing gameplay code and blueprint wrappers for online and platform operations.

## About CommonUser

CommonUser is a comprehensive user management framework from Epic Games that handles online services, platform integration, and user session management. It offers:

- **User Management**: Centralized system for handling user accounts and authentication
- **Platform Integration**: Seamless integration with various gaming platforms (Steam, Epic Games Store, Console platforms)
- **Online Services**: Wrappers for online subsystem operations
- **Session Management**: User session lifecycle and state management
- **Blueprint Support**: Blueprint-friendly wrappers for C++ functionality

## Original Source

This plugin originates from Epic Games' **Lyra Sample Game**:
- **Project Repository**: https://github.com/EpicGames/UnrealEngine/tree/ue5-main/Samples/Games/Lyra
- **Original Location**: `LyraStarterGame/Plugins/CommonUser`
- **Author**: Epic Games
- **License**: Unreal Engine EULA

## Plugin Description

*Provides gameplay code and blueprint wrappers for online and platform operations.*

This plugin serves as a bridge between Unreal Engine's online subsystem and game-specific functionality, providing:

- **CommonUserSubsystem**: Main subsystem for user management operations
- **CommonSessionSubsystem**: Session management and multiplayer functionality
- **AsyncAction_CommonUserInitialize**: Async operations for user initialization
- **CommonUserTypes**: Type definitions and data structures for user management

## Key Features

- **Multi-Platform Support**: Unified interface for different gaming platforms
- **User Authentication**: Handle login, logout, and user validation
- **Session Management**: Create, join, and manage multiplayer sessions
- **Async Operations**: Non-blocking operations for online services
- **Blueprint Integration**: Easy-to-use Blueprint nodes for designers
- **Error Handling**: Comprehensive error handling for online operations

## Dependencies

This plugin typically works with:
- **OnlineSubsystem**: Unreal Engine's online services framework
- **Engine Core**: Core Unreal Engine systems
- **CommonUI**: Epic's UI framework (for user interface integration)
- **Platform-Specific SDKs**: Steam SDK, Epic Online Services, Console SDKs

## Core Components

### CommonUserSubsystem
- Central management system for user operations
- Handles user initialization and authentication
- Manages user state and profile information
- Provides unified interface across platforms

### CommonSessionSubsystem  
- Multiplayer session creation and management
- Join/leave session operations
- Session search and discovery
- Platform-specific session handling

### Async Actions
- **AsyncAction_CommonUserInitialize**: User initialization workflows
- Non-blocking operations with callback support
- Blueprint-compatible async operations

## Usage Scenarios

CommonUser is essential for games that need:

1. **Multi-Platform Release**: Games shipping on multiple platforms (PC, Console, Mobile)
2. **Online Multiplayer**: Games with multiplayer functionality
3. **User Profiles**: Games that save user progress and settings online
4. **Cross-Platform Play**: Games supporting cross-platform multiplayer
5. **Platform Services**: Integration with platform-specific features (achievements, friends, etc.)

## Integration with Common Framework

This plugin is part of Epic's comprehensive "Common" plugin ecosystem:
- **CommonUI**: Core UI framework for scalable interfaces
- **CommonInput**: Platform-agnostic input handling
- **CommonGame**: Gameplay classes and UI management
- **CommonLoadingScreen**: Loading screen management

## Best Practices

- **Initialize Early**: Initialize user systems during game startup
- **Handle Failures**: Always handle online operation failures gracefully
- **Platform Testing**: Test on all target platforms for platform-specific behavior
- **Async Operations**: Use async operations to prevent blocking the game thread
- **Error Messaging**: Provide clear error messages for users

## Credits

- **Epic Games**: Original creator of the CommonUser plugin as part of Lyra Sample Game
- **Lyra Team**: Development team behind the Lyra Sample Game template
- **Online Services Team**: Unreal Engine team responsible for online subsystem integration