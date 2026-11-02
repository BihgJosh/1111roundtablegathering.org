# Transparent logo assets

The seven transparent PNGs are saved in `public/resources/project-logos/`, alongside the original JPEG references. They were prepared with the built-in imagegen tool, using one background-extraction call per original logo.

Assets: bank-of-welfare.png, bridge.png, manus-dei-christian-centre.png, manus-dei-emblem.png, mission-hope-and-light.png, priesthood-assembly.png, project-i-can.png.

## Prompt used for each source

Use case: background-extraction. Extract the supplied existing company logo onto a genuinely transparent background. Remove only the flat white/light gray or black background, including background inside letter counters and gaps. Preserve ALL original lettering, spelling, shapes, colors, gradients and brand artwork exactly; do not redesign or add anything. Keep black lettering and dark blue details opaque. Tightly frame the complete logo with small even transparent padding, no clipping, no extra whitespace. This is a production website logo asset.

## Display and validation

Initiative logos use a centered 160px-high frame, a 260px maximum width and a 140px maximum height, retaining their intrinsic aspect ratios. The company emblem uses a contained 48px square. Image width and height attributes match the PNG dimensions.

All PNGs have alpha channels and fully transparent pixels. All nine image instances loaded in the production preview. Desktop cards were visually reviewed, and the 390px mobile check confirmed the logos fit their containers without horizontal page overflow. `npm run build` and `git diff --check` passed. The build reports existing gallery-script and missing event-artwork warnings unrelated to the logo changes.
