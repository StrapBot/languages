# StrapBot languages
This is the repository where StrapBot translations are stored.

## Files
### Language data path
```
.
└── xx
    └── __data__.json

./xx/__data__.json
```
#### Example:
```
.
└── en
    └── __data__.json

./en/__data__.json
```

### Choices for application commands path
```
.
└── xx
    └── choices.json

./xx/choices.json
```
#### Example:
```
.
└── en
    └── choices.json

./en/choices.json
```

### Cogs data path
```
.
└── xx
    └── cogs
        └── YourCogClassNameHere
            ├── __data__.json
            └── __description__.md

./xx/cogs/YourCogClassName/__data__.json
./xx/cogs/YourCogClassName/__description__.md
```
#### Example:
```
.
└── en
    └── cogs
        └── Utilities
            ├── __data__.json
            └── __description__.md

./en/cogs/Utilities/__data__.json
./en/cogs/Utilities/__description__.md
```

### Cog commands path
```
.
└── xx
    └── cogs
        └── YourCogClassNameHere
            └── your_command_name_here.json

./xx/cogs/YourCogClassNameHere/your_command_name_here.json
```
#### Example:
```
.
└── en
    └── cogs
        └── Utilities
            └── ping.json

./en/cogs/Utilities/ping.json
```

### Cog group commands path
```
.
└── xx
    └── cogs
        └── YourCogClassName
            └── your_group_command
                ├── __data__.json
                ├── your_subcommand.json
                └── another_subcommand_group
                    ├── __data__.json
                    └── third_subcommand.json

./xx/cogs/YourCogClassName/your_group_command/__data__.json
./xx/cogs/YourCogClassName/your_group_command/your_subcommand.json
./xx/cogs/YourCogClassName/your_group_command/another_subcommand_group/__data__.json
./xx/cogs/YourCogClassName/your_group_command/another_subcommand_group/third_subcommand.json
```

### Commands without cog path
###### This is implemented but it's not being used at the moment.
```
.
└── xx
    └── commands
        └── your_command_name_here.json
```

### Group commands without a cog path
###### This is implemented but it's not being used at the moment.
```
.
└── xx
    └── commands
        └── your_group_command
            ├── __data__.json
            ├── your_subcommand.json
            └── another_subcommand_group
                ├── __data__.json
                └── third_subcommand.json

./xx/commands/your_group_command/__data__.json
./xx/commands/your_group_command/your_subcommand.json
./xx/commands/your_group_command/another_subcommand_group/__data__.json
./xx/commands/your_group_command/another_subcommand_group/third_subcommand.json
```

## Notes
- A group's `__data__.json` is the same as a command's .json file.
- Commands `aliases` depend on the language used.
- - This means the aliases can be also in other languages, but those will work only when the language is set.
- When editing `__description__.md`, keep in mind that:
- - Discord doesn't have full Markdown support.
- - The first line of the file is the short description of the cog.
