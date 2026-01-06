# Features

The **Single Player Tarkov (SPT) Server** is a standalone application that replicates the backend services of official *Escape from Tarkov* servers, enabling a complete offline single-player experience. It provides all essential game systems while allowing extensive customization and modding support.

## Core Capabilities

- **Complete Offline Gameplay**: Full single-player experience without requiring connection to official EFT servers
- **Profile Management**: Create, load, and manage player profiles with automatic backup system
- **Quest System**: All vanilla quests with progression tracking, including dynamic repeatable quests
- **Trader Ecosystem**: Complete trader system with loyalty levels, restocking timers, and dynamic pricing
- **Ragfair Marketplace**: Fully functional flea market with price algorithms, taxes, and offer management
- **Hideout Management**: All hideout areas with upgrading system, resource consumption, and crafting stations
- **Insurance System**: Item insurance mechanics with configurable return timers

## Advanced Game Systems

### Bot & AI
- **Adaptive Bot Difficulty**: Configurable bot difficulty levels that adjust based on player progression
- **Procedural Loadouts**: Bots receive randomized but role-appropriate weapons, gear, and inventory
- **Player Scav System**: Scav runs with configurable cooldown timers and extraction probability
- **Special Events**: Cultist rituals, BTR routes, and airdrop events with configurable spawn parameters

### Locations & Economy
- **Dynamic Loot System**: Map-specific loot tables with container and loose loot placement
- **Weather System**: Realistic day/night cycles with dynamic weather conditions (sunny, cloudy, rainy)
- **Session Economy**: Configurable item value multipliers, trader buy/sell rates, and currency exchange
- **Location-Specific Settings**: Custom bot caps, spawn points, and loot modifiers for each map

## Technical Foundation

- **Built with .NET 9.0**: Modern C# implementation providing excellent performance and stability
- **HTTP/WebSocket API**: Full replication of official server endpoints with secure communication
- **NoGC Region Optimization**: Advanced memory management to minimize performance interruptions
- **Multi-Platform Support**: Windows-focused with Linux compatibility (experimental)

## Modding & Extensibility

- **Dynamic Mod Loading**: Load/unload mods without server restart via the `user/mods` directory
- **Dependency Injection Support**: Mods can integrate with the server's service architecture
- **Runtime Patching**: Modify existing server behavior without source code changes
- **Blazor UI Integration**: Create custom admin interfaces and in-game UI elements
- **Mod Validation System**: Automatic dependency checking and compatibility verification

## Developer Experience

- **IDE Support**: Full debugging capabilities in Visual Studio (17.13.5+) and JetBrains Rider (2024.3+)
- **Configuration-Driven**: Extensive JSON configuration system for server behavior tuning
- **CSharpier Formatting**: Consistent code style enforced through automatic formatting
- **Comprehensive Testing**: Unit test suite covering core game systems and API endpoints

## Performance & Reliability

- **Smart Caching**: Bot loot pools, weather forecasts, and item metadata cached for performance
- **Automatic Recovery**: Profile corruption detection and automatic repair mechanisms
- **Resource Management**: Configurable memory limits and performance thresholds
- **Session Integrity**: Raid state preservation with automatic recovery from unexpected shutdowns
