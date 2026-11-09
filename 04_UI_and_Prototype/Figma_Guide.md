# WICKLIGHT – Figma Guide

## The Figma link

**Figma project and prototype:** ______________________ *(paste your Figma share link here)*

## How to open the Figma prototype

1. Open the Figma link in your web browser. You do not need a Figma account to look at it.
2. Click **Present (▶)** at the top right.
3. The prototype starts on the **Main Menu**.
4. Use the **mouse** to click.

**Important:** in Present mode, Figma uses the arrow keys and the spacebar to go to the next screen. They are not the game controls here. Please use the mouse.

## What is in the Figma file

There are 4 frames. Each frame is 1920 × 1080 and has one screen picture from `screens/`.

| Frame | Picture |
|---|---|
| Main Menu | `screens/01_main_menu.png` |
| Gameplay | `screens/02_gameplay.png` |
| Victory | `screens/03_victory.png` |
| Game Over | `screens/04_game_over.png` |

On top of the pictures there are 11 click areas (invisible boxes). Each one is a link to another frame. The link is **On click → Navigate to**, with a **Dissolve** animation of **150 ms**.

| Frame | Click area | X | Y | W | H | Goes to |
|---|---|---:|---:|---:|---:|---|
| Main Menu | PLAY | 710 | 430 | 500 | 95 | Gameplay |
| Gameplay | Exit door | 1740 | 750 | 120 | 180 | Victory |
| Gameplay | Moth 1 | 1140 | 420 | 160 | 120 | Game Over |
| Gameplay | Moth 2 | 1400 | 820 | 160 | 120 | Game Over |
| Gameplay | Spikes 1 | 480 | 850 | 160 | 70 | Game Over |
| Gameplay | Spikes 2 | 960 | 850 | 240 | 70 | Game Over |
| Gameplay | Spikes 3 | 1280 | 850 | 80 | 70 | Game Over |
| Victory | REPLAY | 510 | 800 | 430 | 95 | Gameplay |
| Victory | MAIN MENU | 980 | 800 | 430 | 95 | Main Menu |
| Game Over | RETRY | 510 | 800 | 430 | 95 | Gameplay |
| Game Over | MAIN MENU | 980 | 800 | 430 | 95 | Main Menu |

X and Y are measured from the top-left corner of the frame. SETTINGS and EXIT have no link.

## Test list

In Present mode, click and tick each line:

- [ ] It starts on the **Main Menu**.
- [ ] PLAY → Gameplay
- [ ] Exit door → Victory
- [ ] Victory: REPLAY → Gameplay
- [ ] Moth 1 → Game Over
- [ ] Game Over: RETRY → Gameplay
- [ ] Moth 2 → Game Over
- [ ] Game Over: MAIN MENU → Main Menu
- [ ] Spikes 1, Spikes 2 and Spikes 3 → Game Over
- [ ] Victory: MAIN MENU → Main Menu

Tip: if you click on a place that is not a link, Figma shows all the click areas in blue.

## How to share the Figma file

1. Click **Share** (top right).
2. Under **Who has access**, choose **Anyone with the link** and **can view**.
3. Click **Copy link**.
4. Paste the link at the top of this page and in `05_Documentation/Submission_Document.md`.
5. Open the link in a private browser window (not logged in). If you can see the file, your teacher can see it too.

## How to make the Figma file again (only if needed)

1. In Figma, make a new **Design** file.
2. Press **F** (Frame tool) and make 4 frames, 1920 × 1080 each. Name them Main Menu, Gameplay, Victory and Game Over.
3. Drag each screen picture from `screens/` into its frame. Set it to **X 0, Y 0, W 1920, H 1080**. Lock it.
4. Press **R** (Rectangle tool) and draw the 11 click areas from the table above. Set the **Fill** opacity to **0%**.
5. Open the **Prototype** tab on the right. For each click area, drag the **+** circle to the frame in "Goes to". Choose **On click → Navigate to**, **Dissolve**, **150 ms**.
6. Click on an empty part of the canvas. Under **Flow starting point**, click **+** and choose **Main Menu**.
7. Test it with the test list above.
