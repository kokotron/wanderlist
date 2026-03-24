Initial push was the result of the following prompt (more or less) in Claude (Free, Sonnet 4.6), on March 24th, 2026, which already provided a very beautiful and usable website.

_A webpage which is basically a world map, with the ability to search for places, and add pins at places, as a to-do list. I will be hosting on github and I want to be able to use it from anywhere (home pc, office pc, phone)._

**Features**
=
• Click anywhere on the map to drop a pin (or search → click a result)\
• 8 categories with color-coded pins (Nature, City, Food, Beach, History, Art, Adventure, Other)\
• To-go / Visited toggle with strikethrough in the sidebar\
• Sidebar filter — All / To go / Visited\
• JSON export/import as a local backup fallback\
• Works on mobile too (sidebar slides to bottom)\


**How cross-device sync work**
=
It uses GitHub Gist as a free sync backend — your own GitHub account stores the data as a private Gist. Setup takes ~2 minutes:\

• Go to github.com → Settings → Developer settings → Personal access tokens → Tokens (classic)\
• Generate a new token with only the gist scope\
• In the app click ⚙ Settings, paste your token, save\
• Click ⇅ Sync — it creates the Gist automatically and shows the Gist ID\

After that, every time you add/edit/delete a place it auto-saves to Gist. On any other device, open the app, enter the same token + Gist ID, and it pulls your data.
