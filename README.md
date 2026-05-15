<!DOCTYPE html>
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
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow: hidden;
      backdrop-filter: blur(10px);
      -webkit-backdrop-filter: blur(10px);
    }

    details.card[open] {
      border-color: rgba(216,240,59,0.35);
    }

    summary {
      list-style: none;
      cursor: pointer;
      padding: 22px 18px;
      display: flex;
      align-items: center;
      gap: 12px;
    }

    summary::-webkit-details-marker {
      display: none;
    }

    .summary-emoji {
      font-size: 22px;
      line-height: 1;
      flex: 0 0 auto;
    }

    .card-title {
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 10px;
      font-size: 21px;
      font-weight: 800;
      line-height: 1.35;
      letter-spacing: -0.03em;
      word-break: keep-all;
    }

    .chevron {
      flex: 0 0 auto;
      font-size: 18px;
      line-height: 1;
      opacity: 0.75;
      transition: transform 0.2s ease;
    }

    details[open] .chevron {
      transform: rotate(180deg);
    }

    .card-body {
      padding: 0 18px 18px;
      border-top: 1px solid rgba(255,255,255,0.08);
    }

    .intro {
      margin: 14px 0 10px;
      padding: 12px 14px;
      border-radius: 16px;
      background: rgba(255,255,255,0.05);
      color: var(--muted);
      font-size: 16px;
      font-weight: 700;
      line-height: 1.6;
      letter-spacing: -0.02em;
      word-break: keep-all;
    }

    .section {
      margin-top: 12px;
    }

    .label {
      display: inline-block;
      font-size: 11px;
      font-weight: 800;
      color: #0c1624;
      background: var(--accent);
      padding: 6px 9px;
      border-radius: 999px;
      margin-bottom: 8px;
      letter-spacing: -0.02em;
    }

    ul, ol {
      margin: 0;
      padding-left: 18px;
    }

    li {
      font-size: 16px;
      font-weight: 700;
      line-height: 1.6;
      color: var(--text);
      margin-bottom: 6px;
      letter-spacing: -0.02em;
      word-break: keep-all;
    }

    .note {
      display: grid;
      gap: 8px;
      margin-top: 12px;
      padding: 12px 14px;
      border-radius: 16px;
      background: rgba(143,227,255,0.08);
      border: 1px solid rgba(143,227,255,0.14);
    }

    .note p {
      margin: 0;
      font-size: 16px;
      font-weight: 700;
      line-height: 1.6;
      color: var(--muted);
      letter-spacing: -0.02em;
      word-break: keep-all;
    }

    .cta {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      width: 100%;
      margin-top: 14px;
      border: none;
      border-radius: 16px;
      padding: 14px 16px;
      font-size: 15px;
      font-weight: 800;
      letter-spacing: -0.02em;
      background: var(--button);
      color: var(--button-text);
      text-decoration: none;
    }

    .footer-tip {
      padding: 2px 4px 0;
      font-size: 12px;
      line-height: 1.5;
      color: var(--soft);
      letter-spacing: -0.02em;
      text-align: center;
    }
  </style>
</head>
<body>
  <main class="wrap">
    <section class="hero">
      <p class="eyebrow"></p>
      <h1>내 첫 포스팅,<br>이대로만 쓰면 돼요</h1>
      <p>아주 잘 쓸 필요도, 길게 쓸 필요도 없어요. <br>예시 하나 고르고 바로 따라 써보세요.</p>
    </section>

    <section class="stack">
      <details class="card">
        <summary>
          <span class="summary-emoji">🏨</span>
          <span class="card-title">
            최근 다녀온 숙소 후기 쓰기
            <span class="chevron">▾</span>
          </span>
        </summary>

        <div class="card-body">
          <div class="intro">여행 글은 이미 다녀온 경험만 있어도 시작하기 쉬워요. <br>최근 다녀온 숙소 하나를 떠올려 보세요.</div>

          <div class="section">
            <span class="label">제목 예시</span>
            <ul>
              <li>제주 애월 오션뷰 숙소 2박 후기, 위치와 가격까지 정리</li>
              <li>오사카 난바 가성비 호텔 추천, 실제 숙박 후기</li>
              <li>강릉 1박2일 숙소 후기, 재방문 의사 있는 이유</li>
              <li>방콕 수영장 호텔 후기, 가족여행 숙소로 괜찮았을까?</li>
              <li>부산 해운대 숙소 추천, 뷰·청결·위치 총정리</li>
            </ul>
          </div>

          <div class="section">
            <span class="label">본문 내용</span>
            <ul>
              <li><strong>서론</strong> : 왜 이 숙소를 예약했는지, 여행 목적과 함께 적기</li>
              <li><strong>본론</strong> : 위치, 객실 상태, 청결, 장점·아쉬운 점, 가격 정리</li>
              <li><strong>결론</strong> : 어떤 사람에게 추천하는지, 다시 갈 의사가 있는지</li>
            </ul>
          </div>

          <div class="note">
            <p><strong>⚠️참고사항</strong> : 처음 숙소 링크를 만든다면 <strong>아고다</strong>를 추천드려요. 가장 많은 크리에이터가 사용하는 프로그램입니다.</p>
            <p><strong>⚠️링크 팁</strong> : 링크는 1번보다 2~3번 넣는 것이 구매 확률을 높여요</p>
          </div>

          <a class="cta" href="#">예시 바로가기</a>
        </div>
      </details>

      <details class="card">
        <summary>
          <span class="summary-emoji">🛒</span>
          <span class="card-title">
            최근 구매한 물건 후기 쓰기
            <span class="chevron">▾</span>
          </span>
        </summary>

        <div class="card-body">
          <div class="intro">일상 글은 최근 구매한 물건 하나만 있으면 바로 시작할 수 있어요. 아래 주제 중 하나를 골라 써보세요.</div>

          <div class="section">
            <span class="label">주제 예시</span>
            <ol>
              <li>원룸 제습기 건조기 LG 위닉스 VS 넥스코 미니제습기</li>
              <li>여름맞이 스트레이트 체형 수영복 고르기 후보 추천</li>
              <li>신생아부터 쓰는 브라운 체온계, 밤에 열 체크 편한 체온계 후기</li>
              <li>자취생 필수템 가성비 좋은 롤팩 매트리스 데코라인 실루나</li>
              <li>스타우브 솥밥 냄비 꼬꼬데 20 원형 주물냄비 3개월 사용 후기</li>
            </ol>
          </div>

          <div class="section">
            <span class="label">본문 내용</span>
            <ul>
              <li><strong>서론</strong> : 왜 이 브랜드, 이 상품을 구매하게 되었는지</li>
              <li><strong>본론(상세 후기)</strong> : 실제로 써보았더니 어땠는지, 장점·아쉬운 점, 가격 등</li>
              <li><strong>결론</strong> : 어떤 사람들에게 추천하고 싶은지 정리</li>
            </ul>
          </div>

          <div class="note">
            <p><strong>참고사항</strong> : ⚠️처음 상품 링크를 만든다면 <strong>'오늘의집'</strong>을 먼저 확인해보세요.</p>
            <p><strong>링크 팁</strong> : ⚠️링크는 1번보다 2~3번 넣는 것이 구매 확률을 높여요</p>
          </div>

          <a class="cta" href="#">예시 바로가기</a>
        </div>
      </details>
    </section>

    <div class="footer-tip">처음 글은 완벽하지 않아도 괜찮아요. 먼저 발행해보는 게 더 중요해요.</div>
  </main>
</body>
</html>
