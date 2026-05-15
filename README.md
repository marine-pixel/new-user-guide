<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover" />
  <title>첫 포스팅 가이드</title>
  <style>
    :root {
      --bg: #0c1624;
      --text: #f4f1eb;
      --muted: rgba(244, 241, 235, 0.72);
      --soft: rgba(244, 241, 235, 0.56);
      --card-border: rgba(255,255,255,0.12);
      --accent: #d8f03b;
      --button: #f4f1eb;
      --button-text: #0c1624;
      --shadow: 0 16px 40px rgba(0,0,0,0.28);
      --radius: 24px;
    }

    * {
      box-sizing: border-box;
    }

    html, body {
      margin: 0;
      padding: 0;
      min-height: 100%;
      background:
        radial-gradient(circle at top left, rgba(143, 227, 255, 0.08), transparent 28%),
        radial-gradient(circle at top right, rgba(216, 240, 59, 0.08), transparent 22%),
        linear-gradient(180deg, #101b2b 0%, var(--bg) 100%);
      color: var(--text);
      font-family: -apple-system, BlinkMacSystemFont, "Apple SD Gothic Neo", "Pretendard", "Noto Sans KR", "Segoe UI", sans-serif;
    }

    body {
      min-height: 100svh;
    }

    .wrap {
      width: 100%;
      max-width: 460px;
      margin: 0 auto;
      min-height: 100svh;
      padding: calc(env(safe-area-inset-top) + 18px) 18px calc(env(safe-area-inset-bottom) + 18px);
      display: flex;
      flex-direction: column;
      gap: 14px;
    }

    .hero {
      padding: 10px 2px 2px;
    }

    .eyebrow {
      margin: 0 0 10px;
      font-size: 12px;
      line-height: 1.35;
      font-weight: 700;
      color: rgba(244,241,235,0.62);
      letter-spacing: -0.02em;
      text-align: center;
    }

    .hero h1 {
      margin: 0;
      font-size: clamp(28px, 8vw, 44px);
      line-height: 1.08;
      letter-spacing: -0.04em;
      font-weight: 800;
      word-break: keep-all;
      text-align: center;
    }

    .hero p {
      margin: 12px 0 0;
      font-size: 14px;
      line-height: 1.5;
      color: var(--muted);
      letter-spacing: -0.02em;
      word-break: keep-all;
      text-align: center;
    }

    .stack {
      display: grid;
      gap: 14px;
    }

    details.card {
      background: linear-gradient(180deg, rgba(255,255,255,0.08), rgba(255,255,255,0.06));
      border: 1px solid var(--card-border);
