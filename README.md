# Bendcress 1.0 TEST
Native Android Ichimaga one-bend network puzzle. Android 8+ (min26), target35. Package com.gg007.bendcress. Twelve original unique boards on a compact 4x4 lattice.

## Rules
Standard Ichimaga training puzzle on a 4x4 lattice with six numbered circles. Tap a gap between adjacent points to toggle one edge. Join every circle into one connected network. A number counts the full paths ending at that circle, NOT edges or distance. Each path between successive circles is straight or makes at most one right-angle turn. Never pass through another circle without ending a path there. Paths cannot cross, touch, share an edge or branch at ordinary points. Branching at circles is allowed. Equal numbers MAY connect, and cycles ARE allowed: this is standard, non-magnetic and non-crossing Ichimaga. Unused ordinary points are allowed. Every circle in this edition has an exact number; blank-circle clues are omitted. Twelve original unique boards; auto-check after every edge, unlimited undo/reset, next and level selection. Saved palette and optional a-p point guides.

## Download and status
https://mega.co.nz/#!NdkxzBhb!ryoAoaxk9ckgrnw9Eb85skXLubOKfG1zIfTkZX3vifw
APK SHA256 fdf4ec117ccc47d233be08dc87d0c7aa0d202d9ac4e9e0f4522f78b555622878; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Independent DFS enumerates every straight or single-turn path by walking the lattice, then a union-find/degree oracle compares against production adjacency tracing in 311,584 cases. This includes all compatible path subsets on twelve boards and 300,000 seeded random edge masks. Each board has exactly one full-rule solution, including cycles and paths between equal numbers where valid. Explicit cycle/equal-number acceptance and two-bend, non-circle crossing, repeated-circle return and disconnected degree-matching rejection fixtures pass. Bounds, invalid data, undo, solved lock, reset and replay pass. Archived portable generator reproduces all twelve boards and the archived Java oracle reruns with byte-equal source. Actual drawing-adapter gap taps, solve/undo/replay, next, levels, menu, privacy and saved palette/point guides pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 178 prior studio mechanics and web registry game/mechanic records for functional overlap. Islespan connects islands with straight single or double bridges. Glowwillow traces beams with individual turn counts and directed starts. Bendcress instead plans an undirected degree-counted network with arbitrary path lengths, at most one bend per circle-to-circle path, branching only at circles and cycles allowed. Its grid-edge interaction and independent path/graph validation differ from those mechanics. No Ichimaga match found in the reviewed corpus; recovered repository corpus remains partial. Known Ichimaga adaptation, not a global invention claim. Original generated boards, code and visuals; no source puzzle layouts, code or art copied.
Rules https://www.cross-plus-a.com/html/cros7ichm.htm ; independent rules https://www.keepitsimplepuzzles.com/how-to-solve-ichimaga-puzzles/ .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/bendcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.bendcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Bendcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, point guides and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 179-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/gbu17w25ueo5-bendcress-source-archive . Repository https://github.com/iLanis-agent/bendcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
