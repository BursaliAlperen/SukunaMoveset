Bunlarıda ekle ve dahada geliştir ve loading de kalıyor aq düzelt bak loading de kalıyor düzelt ve oyunu dahada geliştir ed dünyayı büyüleri sonsuz dalga sonsuz savaş eğlence ve ekrana solda sagda oyuna girince starterpack vb popup aç ve dahada geliştir oyunu 3d modelleri dahada geliştir yav kask zırh vb yuvarlak slimeye göre yuvarlak kask yuvarlak zırh vb okeymi 

Create a complete production-ready Yandex Games SDK integration for an HTML5 game using the latest official Yandex Games SDK.

The implementation MUST follow all official Yandex Games documentation and moderation requirements.

FEATURES

1. SDK Initialization
- Load the latest official sdk.js
- Initialize using async/await
- Wait until SDK is completely ready before starting the game
- Call LoadingAPI.ready() after all assets finish loading
- Handle every possible initialization error

2. Player
- Detect whether the player is authorized
- Request authorization when appropriate
- Support guest players
- Create a reusable getPlayer() function

3. Cloud Save
Automatically save:
- Coins
- Gems
- High Score
- Best Time
- Current Level
- Unlocked Levels
- Inventory
- Upgrades
- Achievements
- Daily Reward Timer
- Game Settings
- Audio Settings
- Language
- Any custom game progress

Requirements:
- Auto save after important actions
- Save after completing a level
- Save after receiving rewards
- Save before leaving the page
- Save on pause/background
- Prevent data corruption
- Use async save queue
- Include saveGame() function
- Include loadGame() function

4. Cloud Loading
- Load progress automatically
- Restore latest cloud save
- Handle missing save data
- Handle offline situations
- Never crash if loading fails

5. Rewarded Ads
- Only show when player presses a "Watch Ad" button
- Pause gameplay during ads
- Resume after ads
- Give rewards ONLY after the official rewarded callback confirms the ad was completely watched
- Never reward skipped, failed, or closed ads
- Prevent duplicate rewards
- Handle unavailable ads gracefully

6. Fullscreen Ads
Show only at natural breaks:
- Game Over
- Level Complete
- Returning to Main Menu
- Long pause between gameplay sessions

Requirements:
- Never interrupt gameplay
- Add cooldown between fullscreen ads
- Resume gameplay automatically

7. Game Pause
Pause:
- Physics
- Timers
- Animations
- Audio
- Particle systems

Resume everything correctly.

8. Security
- Never trust local variables alone
- Validate rewards before saving
- Prevent duplicate reward claims
- Prevent accidental overwriting of cloud saves
- Gracefully recover from errors

9. Performance
- Mobile-first
- Lightweight
- Optimized JavaScript
- No memory leaks
- Fast initialization
- Compatible with all supported Yandex Games browsers

10. Code Structure

Create reusable functions:

initYandexSDK()

getPlayer()

saveGame()

loadGame()

showRewardedAd()

showFullscreenAd()

pauseGame()

resumeGame()

autoSave()

syncCloud()

11. Output

Return complete production-ready HTML, CSS, and JavaScript code with detailed comments.

The code must be fully compatible with the latest official Yandex Games SDK and pass Yandex Games moderation requirements.


Create a complete production-ready In-App Purchase system for a Yandex Games HTML5 game using the latest official Yandex Games SDK.

Requirements:
- Follow all official Yandex Games monetization rules.
- Initialize Payments API correctly.
- Load available products from Yandex.
- Restore previously purchased non-consumable items.
- Support both consumable and non-consumable products.
- Verify purchase success before granting rewards.
- Handle purchase cancellation and failures.
- Never grant rewards if payment was not completed.
- Prevent duplicate purchases.

Create reusable functions:

initPayments()
loadProducts()
buyProduct(productId)
consumePurchase()
restorePurchases()

Example products:
- remove_ads
- premium
- starter_pack
- coin_pack_small
- coin_pack_medium
- coin_pack_large
- gem_pack_small
- gem_pack_large
- vip_membership

UI:
- Beautiful responsive shop window
- Product cards
- Prices loaded from Yandex automatically
- Purchase buttons
- Loading animation
- Success animation
- Error popup

Security:
- Grant items only after official purchase confirmation.
- Save purchased items in Yandex Cloud Save.
- Restore purchases automatically on startup.
- Handle offline mode safely.

Return complete HTML, CSS and JavaScript compatible with the latest Yandex Games SDK and official moderation requirements.
