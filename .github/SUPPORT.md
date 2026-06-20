# Support & FAQ

Thanks for using **Navarre**! Here's how to get help, and answers to the most common
questions.

## Where to go
- **A question, or "how do I…?"** → **[Discussions](https://github.com/NavarreDR/navarre-repo/discussions)**
  (the friendliest place - ask anything about setup or use).
- **A bug, or a feature request** → **[Issues](https://github.com/NavarreDR/navarre-repo/issues)**
  (please use the templates so I have what I need to reproduce it).

When reporting a bug, it really helps to include: your **Kodi version** (21/Omega?),
your **platform** (Windows / NVIDIA Shield / Fire Stick / other Android), the **skin
version**, and the steps that trigger it.

---

## Installing

**How do I install it?**
1. Download `repository.navarre-x.x.x.zip` from
   **https://navarredr.github.io/navarre-repo/**.
2. Kodi → **Settings → Add-ons → Install from zip file** → pick that zip
   (turn on **Unknown sources** if prompted: *Settings → System → Add-ons → Unknown sources*).
3. **Install from repository → Navarre Repository → Look and feel → Skin → Navarre.**
4. From then on Kodi keeps the skin **up to date automatically**.

**The installer seems to hang for a minute or two.**
That's normal on a fresh Kodi. After you pick the zip, Kodi quietly downloads a few
helper add-ons (skinshortcuts, embuary, etc.) in the background - there's often a
**1-2 minute delay with little on-screen feedback**. Don't re-select the zip or restart
the installer; just wait for the "Add-on installed" notice.

**"Failed to load dependency" / "could not be satisfied"?**
Kodi couldn't reach its add-on repository to fetch a helper add-on - usually a slow
connection on a fresh install, not a problem with the skin. Open **Add-ons → Install from
repository → Kodi Add-on repository** so it refreshes the list, then try again. Installing
via the **Navarre repository** (step 3 above) avoids this.

---

## Setting up your media

**How do I build my menu?**
On the home screen highlight **More**, press **OK**, choose **Set up my media**, then
browse **into** your media folder (the one containing Movies, Television, etc.) and
confirm. The skin builds one menu item per top folder and switches on the poster-wall view.

**Why folders instead of a Kodi "library"?**
Kodi's library mode flattens everything into one big list and loses your folders (your
James Bond collection, your Season folders…). Navarre browses your folders exactly as they
sit on disk, so your organization is preserved.

**I moved to a different drive / my media is somewhere else now.**
**More → Settings → Select my media root folder**, then re-run **Set up my media**.

**On Android / Shield / Fire Stick, where's my media?**
External drives show up under a path like `/storage/XXXX-XXXX/…`. Browse there in
**Set up my media**. (tinyMediaManager only runs on a PC, so curate posters on the PC
first, then copy the small `.nfo/.jpg/.png` files over - the videos can stay put.)

> **Note:** folder paths that contain a **comma** can't be used as menu targets (Kodi's
> internal command syntax splits on commas). The skin will warn you and skip those - just
> rename the folder to remove the comma.

---

## Posters & artwork

**My posters won't update after I edited them in tinyMediaManager.**
Kodi caches artwork **by file path**, so it keeps showing the old image. Use
**More → Settings → Refresh artwork** (clears the texture cache) - or press **Left** on a
folder and choose **Refresh artwork** for just that one. The new art appears after that.

**Some posters are blank right after install.**
Kodi caches artwork the first time a tile is shown - scroll through the folder once and
the tiles fill in. If a tile stays blank, that movie is missing its poster file; fix it in
tinyMediaManager, or use **More → Settings → Fetch artwork & info (TMDB)** (needs a free
TMDB key).

**Concert videos / workout programs have no posters.**
Expected - they aren't in the movie/TV databases. Leave them, or drop your own
`folder.jpg` into those folders.

---

## Look & behaviour

**A web "popular movies" strip appeared on the home screen.**
Re-run **More → Set up my media**, or set a Home background image - either one clears it.

**Something looks wrong / I switched over from Arctic Zephyr and the home is mixed up.**
**More → Settings → Reset to Navarre defaults** re-applies the intended look without
touching your menu or media.

**A change didn't take effect.**
Most changes are instant, but a few (background images, on-screen text) need **one Kodi
restart** because Kodi caches the layout.

**The options blade keeps opening/closing on its own.**
That's mouse-hover near the left edge. On a TV box, turn the mouse off:
**Settings → System → Input → Enable mouse and touch screen support → Off.**

---

## The two gestures worth knowing
- **OK** = open the highlighted thing.
- **Left** = options for the highlighted folder (rename, move, change icon, delete, refresh art).

---

## Donating
Navarre is free and non-commercial (CC BY-NC-SA 3.0). If you'd like to chip in, there's a
**Sponsor** button at the top of the repo and a voluntary link in the skin's menu -
entirely optional.
