{
  "Type": "Charging",
  "DisplayProgress": false,
  "Next": {
    "0": "Weapon_Battleaxe_Primary_Chain",
    "0.2": {
      "Type": "Replace",
      "Var": "Downstrike_StaminaCondition",
      "DefaultOk": true,
      "DefaultValue": {
        "Interactions": [
          "Weapon_Battleaxe_Primary_Downstrike_StaminaCondition"
        ]
      }
    }
  }
}# notes

{
  "Type": "StatsCondition",
  "Costs": {
    "Stamina": 0.1
  },
  "Failed": "Weapon_Battleaxe_Primary_Chain",
  "Next": {
    "Type": "ChangeStat",
    "Behaviour": "Set",
    "StatModifiers": {
      "StaminaRegenDelay": -3
    },
    "Next": {
      "Type": "Replace",
      "Var": "Downstrike",
      "DefaultOk": true,
      "DefaultValue": {
        "Interactions": [
          "Weapon_Battleaxe_Primary_Downstrike"
        ]
      }
    }
  }
}
