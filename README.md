# 🌀 AstridPortals

AstridPortals is a powerful plugin designed to restrict player access to specific portals based on their requirements. By setting up custom configurations, you can ensure that only players who meet certain criteria are allowed to enter designated portals.

## 🔧 Configuration

Below is an example configuration for AstridPortals:

```yaml
worldname:
  # Placeholder to use for dynamic level checks
  placeholder: "%astridlevels%"
  
  # Condition to check against the player's level
  # Options: ">", "<", ">=", "<=", "="
  check: ">="
  
  # The level requirement for accessing the portal
  value: <level_requirement>
  
  # Message displayed to the player if they do not meet the requirement
  failure-message: "You must reach level %astridlevels% to enter this portal."
```

### Configuration Breakdown

- worldname: Replace with the name of the world where the portal is located. You can specify different configurations for each world.

- placeholder: Defines the placeholder to be used for checking player levels. The default placeholder is %astridlevels%, which should be replaced with the appropriate value or variable if needed.

- check: Specifies the condition for the level check. You can use operators like >, <, >=, <=, and = to define the level requirement.

- value: Sets the required level that players must meet to gain access to the portal.

- failure-message: Customize the message displayed to players who do not meet the level requirement. Use %astridlevels% to dynamically display the player's current level in the message.
