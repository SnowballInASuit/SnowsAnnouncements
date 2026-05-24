[snows_announcements_readme.html](https://github.com/user-attachments/files/28186261/snows_announcements_readme.html)

<!DOCTYPE html>
<html>
<head>
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: var(--font-mono); background: transparent; color: var(--color-text-primary); padding: 1rem 0; }
  .readme { max-width: 680px; }
  .badge-row { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 1.5rem; }
  .badge { font-size: 11px; font-weight: 500; padding: 3px 10px; border-radius: 20px; border: 0.5px solid var(--color-border-secondary); color: var(--color-text-secondary); background: var(--color-background-secondary); font-family: var(--font-mono); }
  .badge.green { background: #EAF3DE; color: #3B6D11; border-color: #639922; }
  .badge.blue { background: #E6F1FB; color: #185FA5; border-color: #378ADD; }
  .badge.purple { background: #EEEDFE; color: #534AB7; border-color: #7F77DD; }
  .badge.amber { background: #FAEEDA; color: #854F0B; border-color: #BA7517; }
  .title-block { margin-bottom: 2rem; }
  .plugin-name { font-size: 28px; font-weight: 500; letter-spacing: -0.5px; font-family: var(--font-mono); color: var(--color-text-primary); margin-bottom: 6px; }
  .plugin-name span { color: #534AB7; }
  .tagline { font-size: 15px; color: var(--color-text-secondary); font-family: var(--font-sans); line-height: 1.6; }
  .section { margin-bottom: 2rem; }
  .section-title { font-size: 13px; font-weight: 500; text-transform: uppercase; letter-spacing: 1px; color: var(--color-text-tertiary); margin-bottom: 1rem; padding-bottom: 6px; border-bottom: 0.5px solid var(--color-border-tertiary); font-family: var(--font-mono); }
  .feature-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 10px; }
  .feature-card { background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 12px 14px; }
  .feature-card .icon { font-size: 18px; color: #534AB7; margin-bottom: 6px; }
  .feature-card .f-title { font-size: 13px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 3px; font-family: var(--font-sans); }
  .feature-card .f-desc { font-size: 12px; color: var(--color-text-secondary); line-height: 1.5; font-family: var(--font-sans); }
  .cmd-block { background: var(--color-background-secondary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 14px 16px; margin-bottom: 10px; }
  .cmd { font-size: 13px; font-weight: 500; color: #534AB7; font-family: var(--font-mono); margin-bottom: 4px; }
  .cmd-desc { font-size: 12px; color: var(--color-text-secondary); font-family: var(--font-sans); line-height: 1.5; }
  .perm-row { display: flex; align-items: flex-start; gap: 10px; padding: 8px 0; border-bottom: 0.5px solid var(--color-border-tertiary); font-family: var(--font-sans); }
  .perm-row:last-child { border-bottom: none; }
  .perm-node { font-size: 12px; font-family: var(--font-mono); color: #185FA5; background: #E6F1FB; padding: 2px 8px; border-radius: 4px; white-space: nowrap; }
  .perm-desc { font-size: 12px; color: var(--color-text-secondary); }
  .type-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(120px, 1fr)); gap: 8px; }
  .type-pill { text-align: center; padding: 8px; border-radius: var(--border-radius-md); font-size: 12px; font-weight: 500; font-family: var(--font-mono); border: 0.5px solid; }
  .t-info { background: #E6F1FB; color: #185FA5; border-color: #378ADD; }
  .t-warning { background: #FAEEDA; color: #854F0B; border-color: #BA7517; }
  .t-event { background: #EEEDFE; color: #534AB7; border-color: #7F77DD; }
  .t-update { background: #EAF3DE; color: #3B6D11; border-color: #639922; }
  .t-alert { background: #FCEBEB; color: #A32D2D; border-color: #E24B4A; }
  .size-row { display: flex; gap: 8px; flex-wrap: wrap; }
  .size-pill { padding: 6px 14px; border-radius: 20px; font-size: 12px; font-family: var(--font-mono); border: 0.5px solid var(--color-border-secondary); color: var(--color-text-secondary); background: var(--color-background-secondary); }
  .config-item { display: flex; justify-content: space-between; align-items: flex-start; padding: 7px 0; border-bottom: 0.5px solid var(--color-border-tertiary); font-family: var(--font-sans); }
  .config-item:last-child { border-bottom: none; }
  .config-key { font-size: 12px; font-family: var(--font-mono); color: var(--color-text-primary); }
  .config-val { font-size: 11px; color: var(--color-text-secondary); text-align: right; max-width: 240px; }
  .announce-preview { background: #1a1a2e; border-radius: var(--border-radius-md); padding: 16px 20px; font-family: var(--font-mono); font-size: 12px; line-height: 1.9; }
  .ap-sep { color: #555; }
  .ap-header { color: #ff9800; font-weight: 500; }
  .ap-msg { color: #e0e0e0; }
  .ap-link { color: #64b5f6; }
  .ap-from { color: #888; }
  .ap-react { color: #aaa; }
  .ap-emoji { color: #fff; }
  .install-step { display: flex; gap: 12px; align-items: flex-start; padding: 10px 0; border-bottom: 0.5px solid var(--color-border-tertiary); font-family: var(--font-sans); }
  .install-step:last-child { border-bottom: none; }
  .step-num { width: 22px; height: 22px; border-radius: 50%; background: var(--color-background-info); color: var(--color-text-info); font-size: 11px; font-weight: 500; display: flex; align-items: center; justify-content: center; flex-shrink: 0; margin-top: 1px; }
  .step-text { font-size: 13px; color: var(--color-text-primary); line-height: 1.5; }
  .step-text code { font-family: var(--font-mono); font-size: 12px; background: var(--color-background-secondary); padding: 1px 5px; border-radius: 3px; }
  .footer { margin-top: 2rem; padding-top: 1rem; border-top: 0.5px solid var(--color-border-tertiary); font-size: 12px; color: var(--color-text-tertiary); font-family: var(--font-sans); text-align: center; }
</style>
</head>
<body>
<div class="readme">

  <div class="title-block">
    <div class="plugin-name">❄️ <span>Snows</span>Announcements</div>
    <div class="tagline">A powerful, fully-customizable announcement plugin for Paper 1.21.x — featuring MiniMessage support, clickable reactions, auto-broadcasts, server event hooks, and much more.</div>
  </div>

  <div class="badge-row">
    <span class="badge green">Paper 1.21.11</span>
    <span class="badge blue">Java 21</span>
    <span class="badge purple">MiniMessage</span>
    <span class="badge amber">LuckPerms Ready</span>
    <span class="badge green">Maven</span>
    <span class="badge blue">Hex Colors</span>
  </div>

  <div class="section">
    <div class="section-title">// preview</div>
    <div class="announce-preview">
      <div class="ap-sep">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</div>
      <div class="ap-header">⚠ [ANNOUNCEMENT] ⚠  [EVENT]</div>
      <div class="ap-msg">Make sure to join our Discord server!</div>
      <div class="ap-link">🔗 Click Here  ← discord.gg/example</div>
      <div class="ap-from">— From: SnowballInASuit</div>
      <div class="ap-sep">━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━</div>
      <div class="ap-react">[Reactions] <span class="ap-emoji">👍 3</span>  |  <span class="ap-emoji">❤️ 1</span>  |  <span class="ap-emoji">🎉 5</span>  |  🔥  |  😮</div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">// features</div>
    <div class="feature-grid">
      <div class="feature-card">
        <div class="icon"><i class="ti ti-speakerphone" aria-hidden="true"></i></div>
        <div class="f-title">Rich Announcements</div>
        <div class="f-desc">Chat + screen title simultaneously, or either individually. Configurable per-send.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-palette" aria-hidden="true"></i></div>
        <div class="f-title">MiniMessage + Hex Colors</div>
        <div class="f-desc">Full MiniMessage support including gradients, rainbow, hover/click events, and &#38;/hex colors.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-mood-happy" aria-hidden="true"></i></div>
        <div class="f-title">Clickable Reactions</div>
        <div class="f-desc">Players click emoji reactions in chat. Hover to see who reacted. Fully customizable emoji list.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-clock" aria-hidden="true"></i></div>
        <div class="f-title">Auto-Announcements</div>
        <div class="f-desc">Cycle through a list of messages automatically on a configurable timer.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-history" aria-hidden="true"></i></div>
        <div class="f-title">Announcement History</div>
        <div class="f-desc">Paginated history log with timestamps, sender, type, and target. Optionally saved to file.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-server" aria-hidden="true"></i></div>
        <div class="f-title">Server Event Hooks</div>
        <div class="f-desc">Automatically broadcasts a custom announcement when /stop or /restart is run.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-link" aria-hidden="true"></i></div>
        <div class="f-title">Clickable Links</div>
        <div class="f-desc">Links are clickable in chat with hover preview text. Opens in browser instantly.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-user" aria-hidden="true"></i></div>
        <div class="f-title">Target Specific Players</div>
        <div class="f-desc">Send announcements to a single player using @PlayerName at the end of the command.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-check" aria-hidden="true"></i></div>
        <div class="f-title">Confirm System</div>
        <div class="f-desc">Optional confirm prompt before sending. Cooldown (default 3 min) so you don't have to confirm every time.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-volume" aria-hidden="true"></i></div>
        <div class="f-title">Custom Sounds</div>
        <div class="f-desc">Play any Minecraft sound on announcement. Volume and pitch configurable.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-layout-2" aria-hidden="true"></i></div>
        <div class="f-title">5 Title Sizes</div>
        <div class="f-desc">XS, S, M, ML, L — each with configurable fade-in, stay, and fade-out durations.</div>
      </div>
      <div class="feature-card">
        <div class="icon"><i class="ti ti-shield" aria-hidden="true"></i></div>
        <div class="f-title">LuckPerms Ready</div>
        <div class="f-desc">Full permission node system, compatible with LuckPerms and any other permissions plugin.</div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">// announcement types</div>
    <div class="type-grid">
      <div class="type-pill t-info">INFO</div>
      <div class="type-pill t-warning">WARNING</div>
      <div class="type-pill t-event">EVENT</div>
      <div class="type-pill t-update">UPDATE</div>
      <div class="type-pill t-alert">ALERT</div>
    </div>
    <div style="margin-top: 10px; font-size: 12px; color: var(--color-text-secondary); font-family: var(--font-sans);">Each type has its own prefix, chat color, and sound — all editable in config.yml.</div>
  </div>

  <div class="section">
    <div class="section-title">// title sizes</div>
    <div class="size-row">
      <span class="size-pill">XS — extra small</span>
      <span class="size-pill">S — small</span>
      <span class="size-pill">M — medium</span>
      <span class="size-pill">ML — med-large</span>
      <span class="size-pill">L — large</span>
    </div>
  </div>

  <div class="section">
    <div class="section-title">// commands</div>
    <div class="cmd-block">
      <div class="cmd">/announce &lt;type&gt; &lt;size&gt; &lt;message&gt; [link] [@player]</div>
      <div class="cmd-desc">Send an announcement. Optionally include a clickable link and/or target a specific player at the end.</div>
    </div>
    <div class="cmd-block">
      <div class="cmd">/announce-confirm</div>
      <div class="cmd-desc">Confirm a pending announcement. Cooldown timer prevents re-confirming every send.</div>
    </div>
    <div class="cmd-block">
      <div class="cmd">/announce-reload</div>
      <div class="cmd-desc">Reload config.yml live without restarting the server.</div>
    </div>
    <div class="cmd-block">
      <div class="cmd">/announce-history [page]</div>
      <div class="cmd-desc">Browse paginated announcement history with clickable next-page buttons in chat.</div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">// permissions</div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 4px 14px;">
      <div class="perm-row"><span class="perm-node">snowsannouncements.announce</span><span class="perm-desc">Send announcements</span></div>
      <div class="perm-row"><span class="perm-node">snowsannouncements.reload</span><span class="perm-desc">Reload the config (op only by default)</span></div>
      <div class="perm-row"><span class="perm-node">snowsannouncements.history</span><span class="perm-desc">View announcement history</span></div>
      <div class="perm-row"><span class="perm-node">snowsannouncements.admin</span><span class="perm-desc">All permissions combined</span></div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">// config.yml highlights</div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 4px 14px;">
      <div class="config-item"><span class="config-key">display-mode</span><span class="config-val">BOTH / TITLE_ONLY / CHAT_ONLY</span></div>
      <div class="config-item"><span class="config-key">confirm.cooldown-seconds</span><span class="config-val">Seconds before re-confirm needed (default 180)</span></div>
      <div class="config-item"><span class="config-key">prefix</span><span class="config-val">MiniMessage string — fully customizable header</span></div>
      <div class="config-item"><span class="config-key">from-format</span><span class="config-val">Uses {player} placeholder</span></div>
      <div class="config-item"><span class="config-key">reactions.available</span><span class="config-val">List of emoji players can react with</span></div>
      <div class="config-item"><span class="config-key">auto-announce.enabled</span><span class="config-val">Toggle + interval + message list</span></div>
      <div class="config-item"><span class="config-key">server-events.stop/restart</span><span class="config-val">Custom message, type, size, and sound</span></div>
      <div class="config-item"><span class="config-key">history.log-to-file</span><span class="config-val">Save all announcements to announcements.log</span></div>
      <div class="config-item"><span class="config-key">types.*</span><span class="config-val">Per-type prefix, color, and sound override</span></div>
      <div class="config-item"><span class="config-key">title-sizes.*</span><span class="config-val">Per-size fade-in, stay, fade-out in ticks</span></div>
      <div class="config-item"><span class="config-key">messages.*</span><span class="config-val">Every player-facing message is editable</span></div>
    </div>
  </div>

  <div class="section">
    <div class="section-title">// installation</div>
    <div style="background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 4px 14px;">
      <div class="install-step"><div class="step-num">1</div><div class="step-text">Download the latest <code>.jar</code> from Releases</div></div>
      <div class="install-step"><div class="step-num">2</div><div class="step-text">Drop it into your server's <code>plugins/</code> folder</div></div>
      <div class="install-step"><div class="step-num">3</div><div class="step-text">Start or restart your Paper 1.21.x server</div></div>
      <div class="install-step"><div class="step-num">4</div><div class="step-text">Edit <code>plugins/SnowsAnnouncements/config.yml</code> to your liking</div></div>
      <div class="install-step"><div class="step-num">5</div><div class="step-text">Run <code>/announce-reload</code> to apply changes live</div></div>
    </div>
  </div>

  <div class="footer">Made with ❤️ by SnowballInASuit &nbsp;·&nbsp; Paper 1.21.x &nbsp;·&nbsp; Java 21 &nbsp;·&nbsp; MIT License</div>

</div>
</body>
</html>
