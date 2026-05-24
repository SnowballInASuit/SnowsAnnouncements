❄️ SnowsAnnouncements
SnowsAnnouncements is a feature-rich announcement plugin built for Paper 1.21.11 Minecraft servers. It gives server owners and staff complete control over how announcements are sent to players, with deep customization for every single feature through a well-organized config.yml. Whether you're running a small private server or a large public network, this plugin scales to fit your needs perfectly.

📢 Announcements
When you send an announcement, it displays a fully framed message in chat surrounded by customizable separator lines, with a header prefix (default ⚠ [ANNOUNCEMENT] ⚠), the message body, an optional clickable link, and a "From: [player]" line at the bottom showing exactly who sent it. Announcements can also display as a large title and subtitle directly on every player's screen at the same time, or you can choose to show only the chat message, only the screen title, or both together. This is controlled globally in the config but can be changed anytime.

🎨 Color & Formatting Support
SnowsAnnouncements has full MiniMessage support, which is the modern Paper formatting system. This means you can use gradients, rainbow effects, hover text, click events, bold, italic, underline, strikethrough, and obfuscated text anywhere in your messages. Hex colors are fully supported using the &#RRGGBB format, giving you access to over 16 million colors instead of just the 16 basic Minecraft colors. Legacy & color codes work too for simplicity.

🏷️ Announcement Types
Every announcement is sent with a type that controls its visual style and sound. There are five built-in types: INFO for general information, WARNING for important notices, EVENT for server events like giveaways or games, UPDATE for plugin or server updates, and ALERT for urgent messages. Each type has its own colored prefix shown in chat, its own chat text color, and its own sound that plays when the announcement fires. Every single one of these is fully editable in the config, and you can even add brand new types with any name, color, prefix, and sound you want.

📏 Title Sizes
When an announcement appears as a title on screen, you choose the size. There are five sizes: XS for extra small, S for small, M for medium, ML for medium-large, and L for large. Size controls how long the title stays on screen and how long it takes to fade in and fade out, all measured in ticks (20 ticks equals one second). Every size has fully configurable fade-in, stay, and fade-out durations in the config so you can tune exactly how long each one lingers on screen.

🔗 Clickable Links
You can attach a link to any announcement by including it in the command. The link appears in chat as a clickable 🔗 Click Here button. Hovering over it shows a preview of the full URL before clicking. When clicked it opens directly in the player's browser. The format of the link button, the hover text, and the display text are all customizable in the config.

😄 Reactions
After every announcement is sent to the whole server, a reaction bar appears in chat below it. Players can click any emoji to react to the announcement. Hovering over a reaction shows a list of every player who has reacted with that emoji. If a player clicks a different emoji their previous reaction switches over automatically. The list of available emojis is fully customizable in the config, the format of the reaction bar is customizable, and you can toggle the whole system on or off. Reactions only appear on server-wide announcements and not on announcements targeted at a specific player.

✅ Confirm System
To prevent accidental announcements, the plugin includes an optional confirmation step. When you run /announce, instead of sending immediately it shows you a prompt asking you to confirm by running /announce-confirm within a short time window (default 10 seconds) before it expires. To avoid making this annoying when sending lots of announcements back to back, there is a cooldown on the confirmation (default 3 minutes). Once you confirm once, the plugin remembers that for the cooldown duration and sends future announcements immediately without asking again. The cooldown duration, the expiry window, and the prompt message are all configurable.

👤 Target Specific Players
By default announcements go to every online player. If you want to send one to a specific player only, add @PlayerName at the very end of the command. The announcement will be sent exclusively to that player in chat and on their screen, and reactions will not appear since it's a private announcement. If the target player is not online you get a clear error message.

🔊 Custom Sounds
Every announcement plays a sound to all recipients when it fires. The default sound is ENTITY_ENDER_DRAGON_GROWL for a dramatic feel. The sound, volume, and pitch are all configurable in the config. Each announcement type can also override the global sound with its own unique sound, so INFO could play a soft pling while ALERT plays the dragon roar.

⏱️ Auto-Announcements
The plugin can automatically broadcast messages on a repeating timer without anyone having to type a command. You set up a list of messages in the config and an interval in seconds, and the plugin cycles through them one by one, looping back to the start when it reaches the end. Auto-announcements have their own type, size, and display mode settings separate from manual announcements, so you can have them show only in chat while manual announcements show on screen too.

📜 Announcement History
Every announcement that gets sent is logged to an in-memory history with a timestamp, the sender's name, the type, the message, and the target if there was one. Staff can browse this history with /announce-history which shows it in a paginated list with clickable next-page buttons right in chat. The history can also be saved to a log file on disk so it persists even after server restarts. The maximum number of entries kept, the log file name, and every message format in the history display are all configurable.

🖥️ Server Stop & Restart Hooks
When an operator or console runs /stop or /restart, SnowsAnnouncements automatically fires a big announcement to all online players warning them what is about to happen. The stop and restart announcements are completely separate from each other with their own message, type, size, and sound each fully configurable in the config. This gives players a heads-up before the server goes down so they can get to safety.

🔄 Reload Command
You can reload the entire config live at any time without restarting the server by running /announce-reload. This applies every change in config.yml instantly including auto-announce settings, type definitions, sounds, messages, and everything else.

🔐 Permissions & LuckPerms Support
SnowsAnnouncements uses a clean permission node system that works with any permissions plugin including LuckPerms. snowsannouncements.announce controls who can send announcements, snowsannouncements.reload controls who can reload the config, snowsannouncements.history controls who can view the history, and snowsannouncements.admin is a parent node that grants all of the above at once. None of these default to true for regular players so you have full control over exactly who can do what.

⚙️ Config.yml
Absolutely everything in this plugin is configurable. The global display mode, the confirm cooldown, the confirmation prompt message, the expiry window, sound settings, the announcement prefix and separator, the from-line format, every title size's timing, every announcement type's prefix and color and sound, the auto-announce list and interval and mode, the reactions emoji list and display format, the history size and log file, the link format, the server stop and restart messages, and every single player-facing message the plugin ever sends. Nothing is hardcoded. If you don't like how something looks or works, it's in the config.

Made with 💙 by SnowballInASuit

