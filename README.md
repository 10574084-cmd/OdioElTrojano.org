# OdioElTrojano.org

A small opt-in video page experiment. One click opens one separate player window; a second click inside the player starts playback and bass-triggered window movement.

## Add your video

The uploaded third-party clip is not included in this public repository. Before publishing any media, make sure you have permission to distribute it publicly.

1. Create the folder `media/`.
2. Add a video you own or have permission to publish as `media/odio-el-trojano.mp4`.
3. Open the site and click **ABRIR VENTANA DEL VIDEO**.
4. In the new window, click **PLAY VIDEO + START JUMP**.

## Controls

- **STOP MOVEMENT** stops the physical window motion and returns it to its starting position; the video can continue.
- **CLOSE WINDOW** pauses the video and closes the popup where the browser allows it.
- The main page opens only one popup, directly in response to a click.

## Browser limitations

Physical window movement is best-effort. Browsers and operating systems may ignore `window.moveTo()`, including on some Linux/Wayland and mobile environments. The page cannot force the browser to move a window.

## GitHub Pages

The workflow in `.github/workflows/deploy.yml` deploys the repository root to GitHub Pages when changes are pushed to `main`. For the first deployment, set **Settings → Pages → Build and deployment → Source → GitHub Actions**.
