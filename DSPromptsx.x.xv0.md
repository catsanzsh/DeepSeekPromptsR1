{
  "environment": {
    "state_space": {
      "player_state": "...", 
      "world_state": "...", 
      "narrative_state": "...", 
      "physics_state": "..."
    },
    "action_space": {
      "player_actions": ["move", "attack", "use_item", "..."],
      "narrative_actions": ["trigger_event", "branch_story", "..."],
      "physics_actions": ["adjust_gravity", "modify_friction", "spawn_weather_effect"]
    }
  },
  "agent": {
    "algorithm": "Deep Q-Network",
    "neural_network": {
      "layers": [128, 128, 128],
      "activation": "ReLU",
      "input": "state_space",
      "output": "action_space"
    },
    "hyperparameters": {
      "learning_rate": 0.001,
      "discount_factor": 0.99,
      "exploration_rate": 0.1
    }
  },
  "rewards": {
    "goal_completion": +100,
    "enemy_defeat": +10,
    "player_death": -50,
    "engagement_bonus": +5,
    "narrative_coherence_bonus": +5,
    "physics_stability_bonus": +2
  },
  "features": [
    "AI-driven narrative design",
    "real-time physics adaptation"
  ]
}
