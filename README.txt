IMPERIAL OCCUPATION -- LOADING SCREEN (0.152)
=============================================
What players see while they connect: the crest, "Welcome to the server",
a progress bar with the file being downloaded, useful commands, a rotating
Imperial directive and a tip for new players. Same colours, crest and fonts
as the in-game interface.

Files:  index.html      the page (all words are in the TEXT block at the bottom)
        fonts/          the fonts the content pack ships (Star Jedi, Roboto
                        Condensed, Share Tech Mono) -- keep them next to the page

WHY IT NEEDS HOSTING
  Garry's Mod shows the loading screen from a WEB ADDRESS (the sv_loadingurl
  setting), not from a file on the server. So this folder has to be put on
  the web once. This repository is private, so GitHub cannot host it from here.

ONE-TIME SETUP (free, about 5 minutes)
  1. On GitHub, create a NEW repository, e.g. "ixempire-loading", PUBLIC.
  2. Upload index.html and the fonts folder into it (Add file -> Upload files,
     drag the whole contents of this folder in).
  3. Settings -> Pages -> Source: "Deploy from a branch", branch main, folder
     / (root), Save. After a minute the page is at
         https://daand1309.github.io/ixempire-loading/
     (open it in a browser to check -- it shows the screen with no progress).
  4. In game: F1 -> Config -> Empire -> loadingScreenURL = that address.
     It applies at once; players who connect after that see it.

  Any other web host works just as well: upload the folder, put its address
  in loadingScreenURL.

CHANGING THE WORDS
  Edit the TEXT block at the bottom of index.html (commands, directives,
  tips), then upload index.html to the hosting repository again. Players
  may need a restart of their game to see a new version (browser cache).
