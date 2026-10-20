# TruthTrace

![TruthTrace logo](assets/logo.png)

TruthTrace is a free fact-check helper for social posts, articles, screenshots and claims. It follows the SIFT method from Mike Caulfield: **Stop**, **Investigate the source**, **Find better coverage**, **Trace claims, quotes and media to the original context**. Every report cites the sources it opened, gives a verdict with a confidence level, and marks anything it could not confirm as UNVERIFIED. It never invents a source.

## Project status: done, pending, uncertain
**Done**
- 2026-10-20: v1.0.0 built and tested: manifest valid JSON, skill frontmatter valid, every file link resolves, example matches the template, and a real check (Great Wall from space) run with live sources (all URLs HTTP 200).

**Pending**
- Marketplace submission: not submitted yet.
- Translated summaries below are machine-made and not reviewed by native speakers. Corrections welcome through an issue.
- Reverse image search depends on tools the user runs; TruthTrace does not ship one.

**Uncertain**
- How well each AI host searches the web: TruthTrace relies on the host's own web access. Without it, TruthTrace can only guide the user through the steps.
- How the listing works on the Grok Bot and Grok side: not described in the publisher terms.

## Quick start
1. Install (see Installation).
2. Ask: "Is this true? 'The Great Wall of China is the only man-made object visible from space.'"
3. Get a SIFT report: verdict, confidence, cited sources, the original, and what is still unverified.

## Installation
Install from this repository: https://github.com/OmnipotentCEOxJenny/truthtrace (Cursor plugin format: `.cursor-plugin/plugin.json`, `skills/`, `rules/`). No dependencies, no API keys, no paid services.

## Testing
1. Ask TruthTrace to fact-check: "You can see the Great Wall of China from space with the naked eye."
2. Expected: verdict False, confidence High, at least two independent sources (for example NASA and Scientific American) with working URLs, the traced original (NASA's account of the 2004 ISS photo), and a "Still unverified" section.
3. Compare with `examples/great-wall-from-space.md`.

## Credits
- Inventor and publisher: Rob Domaine / Omnipotent Media LLC
- Builder: Jenny Echo
- Method: Mike Caulfield, SIFT (The Four Moves), https://hapgood.us/2019/06/19/sift-the-four-moves/ ; *Web Literacy for Student Fact-Checkers* (CC BY 4.0). TruthTrace is independent and not endorsed by him.

## Rob Domaine's four pillars
1. Trustworthy, honest, real data, truthful: never invent; anything unchecked is marked UNVERIFIED.
2. Use only legitimate means: legitimate, proven sources and methods; unreliable sources rejected.
3. Double-check everything: every finding is confirmed by two independent checks, and the report shows both.
4. Stay within the law and rules always: local, county, state, federal and platform rules.

## Components
- `skills/truthtrace-check`: the full SIFT check with verdicts and confidence.
- `skills/truthtrace-check/references/report-template.md`: the report format.
- `skills/trace-to-original`: tracing quotes, statistics, images and changed pages.
- `rules/pillars-and-scope.mdc`: the pillars and scope.
- `examples/great-wall-from-space.md`: a real, sourced example.

## Languages
These summaries are machine-made translations and have not been reviewed by native speakers. The English text is authoritative.

- **Español:** TruthTrace es un plugin gratuito que verifica publicaciones, artículos y afirmaciones con el método SIFT, cita fuentes y marca lo no verificado.
- **Français:** TruthTrace est un plugin gratuit qui vérifie publications, articles et affirmations avec la méthode SIFT, cite ses sources et signale ce qui n'est pas vérifié.
- **Deutsch:** TruthTrace ist ein kostenloses Plugin, das Beiträge, Artikel und Behauptungen mit der SIFT-Methode prüft, Quellen nennt und Ungeprüftes kennzeichnet.
- **Português:** TruthTrace é um plugin gratuito que verifica publicações, artigos e alegações com o método SIFT, cita fontes e marca o que não foi verificado.
- **Italiano:** TruthTrace è un plugin gratuito che verifica post, articoli e affermazioni con il metodo SIFT, cita le fonti e segnala ciò che non è verificato.
- **Nederlands:** TruthTrace is een gratis plug-in die berichten, artikelen en beweringen controleert met de SIFT-methode, bronnen vermeldt en ongeverifieerde punten markeert.
- **Polski:** TruthTrace to darmowa wtyczka, która sprawdza posty, artykuły i twierdzenia metodą SIFT, podaje źródła i oznacza to, co niezweryfikowane.
- **Русский:** TruthTrace — бесплатный плагин, который проверяет посты, статьи и утверждения методом SIFT, указывает источники и отмечает непроверенное.
- **Українська:** TruthTrace — безкоштовний плагін, що перевіряє дописи, статті й твердження методом SIFT, наводить джерела та позначає неперевірене.
- **Türkçe:** TruthTrace, gönderileri, makaleleri ve iddiaları SIFT yöntemiyle doğrulayan, kaynak gösteren ve doğrulanmamış olanı işaretleyen ücretsiz bir eklentidir.
- **العربية:** TruthTrace إضافة مجانية تتحقق من المنشورات والمقالات والادعاءات بطريقة SIFT، وتذكر المصادر وتشير إلى ما لم يتم التحقق منه.
- **עברית:** TruthTrace הוא תוסף חינמי שבודק פוסטים, כתבות וטענות בשיטת SIFT, מצטט מקורות ומסמן מה שלא אומת.
- **فارسی:** TruthTrace افزونه‌ای رایگان است که پست‌ها، مقاله‌ها و ادعاها را با روش SIFT بررسی می‌کند، منابع را ذکر می‌کند و موارد تأییدنشده را علامت می‌زند.
- **हिन्दी:** TruthTrace एक मुफ़्त प्लगइन है जो SIFT विधि से पोस्ट, लेख और दावों की जाँच करता है, स्रोत बताता है और असत्यापित बातों को चिह्नित करता है।
- **বাংলা:** TruthTrace একটি বিনামূল্যের প্লাগইন, যা SIFT পদ্ধতিতে পোস্ট, প্রবন্ধ ও দাবি যাচাই করে, উৎস উল্লেখ করে এবং অযাচাইকৃত বিষয় চিহ্নিত করে।
- **اردو:** TruthTrace ایک مفت پلگ اِن ہے جو SIFT طریقے سے پوسٹس، مضامین اور دعووں کی جانچ کرتا ہے، ذرائع بتاتا ہے اور غیر تصدیق شدہ باتوں کی نشاندہی کرتا ہے۔
- **中文（简体）:** TruthTrace 是一款免费插件，使用 SIFT 方法核查帖子、文章和说法，注明来源并标记未经核实的内容。
- **日本語:** TruthTrace は、SIFT 法で投稿・記事・主張を検証し、出典を示し、未確認の点を明示する無料プラグインです。
- **한국어:** TruthTrace는 SIFT 방법으로 게시물, 기사, 주장을 검증하고 출처를 밝히며 확인되지 않은 내용을 표시하는 무료 플러그인입니다.
- **Bahasa Indonesia:** TruthTrace adalah plugin gratis yang memeriksa unggahan, artikel, dan klaim dengan metode SIFT, mencantumkan sumber, dan menandai yang belum terverifikasi.
- **Tiếng Việt:** TruthTrace là plugin miễn phí kiểm chứng bài đăng, bài báo và tuyên bố bằng phương pháp SIFT, trích dẫn nguồn và đánh dấu điều chưa được xác minh.
- **Kiswahili:** TruthTrace ni programu-jalizi ya bure inayokagua machapisho, makala na madai kwa mbinu ya SIFT, inataja vyanzo na kuweka alama kwa yasiyothibitishwa.

## License
MIT. See `LICENSE`.
