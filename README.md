# Pentocress 1.0 TEST
Native Android Pentopia nearest-ray pentomino puzzle. Android 8+ (min26), target35. Package com.gg007.pentocress. Twelve original unique boards on a compact 5x4 grid.

## Rules
Pentopia shading puzzle on a 5x4 grid. Each side-connected shaded group must have exactly five cells. Each of the twelve free pentomino shapes may be used at most once; rotations and reflections count as the same shape. Different pieces cannot touch, even at a corner. Gold clue cells stay unshaded. N/E/S/W letters list ALL directions with the nearest shaded cell along the four straight row/column rays; equal nearest distances require multiple letters. N=up, E=right, S=down, W=left. Only aligned cells count, not diagonals. Some shapes may be unused. Tap unnumbered cells to shade/clear. Undo/reset, levels and next; saved palette and optional shade dots. No timer or score.

## Download and status
https://mega.co.nz/#!hZMFmYoK!oEaMs6JxsFfwjrw--O2CbueAwsf5OhZ9tpkN3gvL28o
APK SHA256 e34213f13c00e97f957804051c5f73fdb9cf15eb658246efb0fc7c8942671a62; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent coordinate-list components, normalized dihedral coordinate strings and Manhattan-distance ray comparisons agree with production bit-floods, canonical bitshapes and ray stepping on all 1,048,576 shading masks and 12,582,912 board checks. Exactly 1,224 legal shadings exist on this 5x4 grid: 376 single-piece placements and 848 two-piece placements. The portable seed-621109 generator starts from all 376 placements of the twelve free pentominoes, considers every non-touching pair with different shapes, confirms no three pieces fit, then removes clues only while uniqueness holds. Twelve original clue boards each have one solution, all twelve solutions differ, with three or four gold clue cells and at least one tied-direction clue per board. Fixed clues, ties, diagonal exclusion, bounds, shade/clear, undo/reset, solved lock and malformed states pass. Actual drawing-adapter taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/shade dots. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 193 prior live studio descriptions and byte-current 803 web registry entries using functional terms. No Pentopia/pentomino-nearest-arrow match in this partial corpus. Nearcress compares nearest loop edges rather than placing shapes; Statuefern uses a fixed L/T shape bank without nearest-ray clues; Tetrocress partitions every cell into tetromino rooms. Pentocress instead places optional nonrepeated free pentominoes constrained by nearest-shaded-cell directions and corner separation. Known Pentopia adaptation with original generated boards, code and visuals; no copied layouts/code/art or global invention claim. Competition instructions, publisher rules, independent archive and community solution agree on the core constraints. This ordinary Pentopia edition forbids shading clues, unlike Twilight Pentopia; Tetropia and all-piece inventory variants are not used. No history claim.
Rules https://www.gmpuzzles.com/blog/pentopia-rules-and-info/ ; independent rules https://www.logic-puzzles.ropeko.ch/php/db/puzzle.php?id=68 .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/pentocress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.pentocress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Pentocress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, shape marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 194-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/rxvhzw0rbzap-pentocress-source-archive . Repository https://github.com/iLanis-agent/pentocress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
