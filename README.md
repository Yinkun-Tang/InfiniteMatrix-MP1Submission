# Your First Game: An Infinite Matrix
## 1. Complete the Tutorial
* N/A
## 2. Health System
* At the left bottom corner of the screen during the game play, a health bar and a number indicate the current health of the player.
* Health (value) could be increased if player picks up a health pack, and it may also get decreased when player hits any wall or enemy.
* Each health pack pick up will recover 10 points of health for the player.
* Each hit will penalize the player and reduce 10 points of health from their current health.
* When the health become less or equal to 0, either achieved by hitting any wall or hitting any enemy, the player will immediately stop moving forward, and game restart button will appear on the screen.
* When game restarts, the health will be reset to the maximum possible value, so does the health bar UI.
## 3. Score System
* At the left top corner of the screen during the game play, a current score UI will monitor player's playstyle and give score points reward for player's appropriate manipulations (or behaviors).
* Score could be obtained for the following two behaviors:
1. Correctly pass through the trigger zone without hitting the wall mesh component (10 points each)
2. Shoot projectile and hit any enemy, which will destroy both projectile and enemy (50 points each)
* When game restarts, the score will be reset to 0.
## 4. Health Pack
* Health Pack is a collidable object that gets destroyed upon collision with the player or when it reaches its lifespan (which is set to be 5 seconds).
* The appearance of the health pack is a translucent green cross.
* As described previously, the health pack will recover the player's health up to a maximum possible health value.
* Theoretically, only 1/3 tunnels should have health pack generated, and they will be generated around the center part of the tunnel.
* When game restarts, any possibly remained health pack will be destroyed.
## 5. Player Projectile Attacks
* Left mouse click will shoot a projectile from the current location of the player, which has much faster speed compared to the maximum speed of the player.
* Hit on anything will destroy the projectile, or it will destroy itself after a short duration (which is set to be 1 second).
## 6. Enemy
* Enemy is a collidable object that gets destroyed upon collision with the player or the projectiles. It may also destroy itself after its lifespan (which is set to be 5 seconds).
* 1. Collision with Player: Decrease player's current health
  2. Collision with Projectile: Increase player's current score
* The appearance of the enemy is a lazer red colored sphere.
* Theoretically, 1/2 tunnels will have enemy generated, and they will be generated in a larger area compared to health pack generation area.
* When game restarts, any possibly remained enemy will be destroyed.
## 7. Increase Player Speed Over Time
* The player speed will get faster over time, as its initial speed is set to be 1000, the increase speed rate is set to be 40, and the maximum possible speed is set to be 2500.
* When game restarts, the player speed will also be reset to its initial speed value.
## 8. Creative Modification
* Health bar decreases along a gradient of colors.
* Screen flashes red for a short duration on collision with barriers and enemies.
