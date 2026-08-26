# Design System: Yolunu Bul

## 1. Visual Theme & Atmosphere
Yolunu Bul is a calm, optimistic career-discovery interface: editorial clarity with a tactile, human feel. The mood is “well-designed notebook meets modern guidance studio” — confident but not corporate, warm but never childish. Use an asymmetrical, left-led composition with generous white space and small moments of visual surprise. Density 4/10, variance 7/10, motion 5/10. The product should feel trustworthy for a first-time visitor and useful for someone making a serious career change.

## 2. Color Palette & Roles
- **Paper Canvas** (#F7F8F4) — primary background, soft and slightly warm
- **Clean Surface** (#FFFFFF) — cards, inputs, navigation surfaces
- **Deep Ink** (#1F2521) — primary text and headlines; never pure black
- **Graphite Mist** (#68716B) — secondary text, helper copy, metadata
- **Structural Line** (#DDE3DC) — quiet borders and dividers
- **Moss Accent** (#6B8F71) — the single accent for primary CTAs, progress, selection, and focus states
- **Soft Moss Tint** (#E7EFE6) — selected states and subtle supportive surfaces

Do not introduce additional accent colors, neon colors, purple/blue gradients, or warm/cool gray mixing.

## 3. Typography Rules
- **Display:** Space Grotesk — track-tight, weight-driven, expressive without feeling loud
- **Body:** DM Sans — relaxed leading, readable at 16px, max line length 65 characters
- **Mono:** Space Mono — only for progress labels, small statistics, and assessment metadata
- Headline scale should be controlled with clamp; desktop hero around 64px, mobile around 42px.
- Use sentence case. Keep copy direct, humane, and specific; avoid corporate language.

## 4. Component Stylings
- **Buttons:** Moss fill with deep ink text for the primary action. Height 48px minimum, generous horizontal padding, 14px radius. Tactile active state with a subtle 1px translate and slightly darker fill. No glow.
- **Cards:** White surfaces with a 1px structural line and a very soft shadow. Radius 20px. Use elevation only for decision points and result previews; use whitespace and dividers elsewhere.
- **Inputs:** Labels above controls, visible helper text below when useful. Large 52px fields with clear focus ring in Moss Accent. Never use floating labels.
- **Choice tiles:** Icon/illustration area, title, one-line explanation, selected state with Soft Moss Tint and a 2px Moss Accent edge. Keep each tile distinct in content, not only color.
- **Progress:** Thin horizontal progress track with a small numbered label; the current step is visible in plain language.
- **Navigation:** Minimal top navigation with wordmark, two quiet links, and one compact “Teste başla” CTA. On mobile collapse links into a menu.
- **Loading:** Skeleton blocks matching the result layout; no circular spinner.

## 5. Layout Principles
Use a max-width 1240px grid. The landing screen is a split layout: left column carries eyebrow, headline, proof, and CTA; right column carries a collage-like but non-overlapping visual made of an assessment preview, small statistic note, and career path chips. Keep every element in a clear spatial zone. Avoid equal three-column feature rows; prefer a 7/5 split and an asymmetric two-column section. Below 768px, collapse to one column and keep all tap targets at least 44px.

The first screen should include: top nav, a small status eyebrow “Kendin için doğru yönü keşfet”, headline “Bir meslek seçmek değil, sana uyan çalışma biçimini bulmak.”, supporting paragraph, primary CTA “Kısa testi başlat”, a small “8 dakika · ücretsiz” note, and a right-side assessment preview with example match labels such as “Analitik”, “İnsan odaklı”, and “Üretken”.

## 6. Motion & Interaction
Use restrained spring-like transitions around 180–280ms with opacity and transform only. Stagger the hero’s text and preview by 60ms. Choice tiles lift by 2px on hover and settle with a tactile press. Progress updates should animate smoothly. Respect reduced-motion preferences. No bouncing arrows, no perpetual decorative motion, no custom cursor.

## 7. Content Principles
Write in natural Turkish. Avoid “geleceğin”, “devrim niteliğinde”, “kusursuz”, “seamless”, “elevate”, and other generic AI copy. Make the user feel seen without making promises about their future. Use realistic labels: “İnsanlarla çalışmak”, “Bir şeyi çözümlemek”, “Yeni bir şey üretmek”, “Düzen kurmak”.

Assessment questions must be indirect, personal, and slightly surprising. Do not ask users to self-label with obvious career-test questions such as “Elektronik sever misin?”, “Sayısal mısın?” or “İnsanlarla çalışmayı sever misin?”. Instead, use everyday preferences as signals for deeper tendencies. Example prompts:
- “Bir dizide karakter olsaydın, hangisine daha yakın hissederdin?”
- “Bir şarkıyı tekrar tekrar dinlemene en çok ne sebep olur?”
- “Evde tek başına geçireceğin beklenmedik bir boş gün nasıl akar?”
- “Bir şey bozulduğunda ilk refleksin ne olur?”
- “Bir arkadaşın senden yardım istediğinde, genelde ne yaparsın?”
- “Yeni bir şehri gezerken seni en çok ne çeker?”

Use 8–12 questions with varied themes: music, fictional characters, free time, repair instincts, noticing details, social energy, making things, and handling ambiguity. Every answer option should describe a recognizable behavior rather than a job or personality label. After each answer, translate the signal into a quiet internal dimension such as pattern noticing, social orchestration, curiosity, making, patience, or autonomy; never expose simplistic diagnosis to the user.

## 8. Anti-Patterns (Banned)
- No emojis anywhere.
- No Inter font, generic serif fonts, or pure black.
- No neon gradients, purple/blue glow, or oversized gradient text.
- No centered generic hero; use the left-led split composition.
- No equal three-card feature row.
- No overlapping text and images.
- No fake precision such as “%99,9 uyum”.
- No generic placeholder names or corporate SaaS language.
- No filler text like “Scroll to explore”.
- No circular spinner or decorative chart clutter.
