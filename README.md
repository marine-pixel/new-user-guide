<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>내 첫 포스팅, 이대로만 쓰면 돼요</title>
  <style>
    * {
      box-sizing: border-box;
    }

    html, body {
      margin: 0;
      padding: 0;
      background: #f7f9fc;
      font-family: -apple-system, BlinkMacSystemFont, "Apple SD Gothic Neo",
        "Pretendard", "Noto Sans KR", sans-serif;
      color: #111827;
    }

    body {
      min-height: 100vh;
    }

    .wrap {
      width: 100%;
      max-width: 430px;
      margin: 0 auto;
      padding: 20px 16px 24px;
    }

    .hero {
      text-align: center;
      padding: 12px 4px 18px;
    }

    .title {
      margin: 0;
      font-size: 31px;
      line-height: 1.28;
      font-weight: 800;
      letter-spacing: -0.03em;
      color: #111827;
    }

    .subtitle {
      margin: 14px 0 0;
      font-size: 16px;
      line-height: 1.55;
      font-weight: 500;
      color: #5b6475;
      word-break: keep-all;
    }

    .card-list {
      display: flex;
      flex-direction: column;
      gap: 14px;
      margin-top: 6px;
    }

    details.card {
      background: #ffffff;
      border: 1px solid #e6ebf2;
      border-radius: 24px;
      box-shadow: 0 10px 30px rgba(17, 24, 39, 0.05);
      overflow: hidden;
    }

    details.card[open] {
      border-color: #d8e4ff;
      box-shadow: 0 14px 34px rgba(74, 144, 226, 0.10);
    }

    summary {
      list-style: none;
      cursor: pointer;
      padding: 24px 22px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 14px;
    }

    summary::-webkit-details-marker {
      display: none;
    }

    .summary-left {
      display: flex;
      align-items: center;
      gap: 12px;
      min-width: 0;
    }

    .emoji {
      font-size: 26px;
      line-height: 1;
      flex-shrink: 0;
    }

    .card-title {
      font-size: 22px;
      line-height: 1.35;
      font-weight: 800;
      letter-spacing: -0.02em;
      color: #111827;
      word-break: keep-all;
    }

    .arrow {
      flex-shrink: 0;
      font-size: 22px;
      color: #9aa4b2;
      transition: transform 0.2s ease;
    }

    details[open] .arrow {
      transform: rotate(180deg);
    }

    .card-body {
      padding: 0 22px 22px;
      border-top: 1px solid #f0f3f8;
    }

    .section {
      margin-top: 18px;
    }

    .section-label {
      margin: 0 0 10px;
      font-size: 14px;
      font-weight: 800;
      color: #4f79d8;
      letter-spacing: -0.01em;
    }

    .desc-box {
      background: #f8fbff;
      border: 1px solid #e5efff;
      border-radius: 16px;
      padding: 14px 14px 12px;
    }

    .desc-box ul,
    .desc-box ol {
      margin: 0;
      padding-left: 18px;
    }

    .desc-box li {
      font-size: 14px;
      line-height: 1.65;
      color: #334155;
      margin-bottom: 6px;
      word-break: keep-all;
    }

    .desc-box li:last-child {
      margin-bottom: 0;
    }

    .tip {
      margin-top: 12px;
      font-size: 13px;
      line-height: 1.6;
      color: #6b7280;
    }

    .button-wrap {
      margin-top: 18px;
    }

    .btn {
      display: block;
      width: 100%;
      text-align: center;
      text-decoration: none;
      background: #4a90e2;
      color: #ffffff;
      font-size: 15px;
      font-weight: 700;
      padding: 14px 16px;
      border-radius: 14px;
      box-shadow: 0 8px 18px rgba(74, 144, 226, 0.20);
    }

    .btn:hover {
      background: #3d82d3;
    }

    @media (max-width: 390px) {
      .wrap {
        padding: 18px 14px 22px;
      }

      .title {
        font-size: 28px;
      }

      .subtitle {
        font-size: 15px;
      }

      .card-title {
        font-size: 20px;
      }

      summary {
        padding: 22px 18px;
      }

      .card-body {
        padding: 0 18px 18px;
      }
    }
  </style>
</head>
<body>
  <main class="wrap">
    <section class="hero">
      <h1 class="title">내 첫 포스팅,<br>이대로만 쓰면 돼요.</h1>
      <p class="subtitle">
        길게 쓸 필요도 몇시간씩 시간을 쓸 필요도 없어요.<br>
        아래 둘 중 하나를 골라 바로 따라 써보세요.
      </p>
    </section>

    <section class="card-list">
      <details class="card">
        <summary>
          <div class="summary-left">
            <div class="emoji">🏨</div>
            <div class="card-title">최근 다녀온 숙소 후기 쓰기</div>
          </div>
          <div class="arrow">⌄</div>
        </summary>

        <div class="card-body">
          <div class="section">
            <p class="section-label">[제목 예시]</p>
            <div class="desc-box">
              <ol>
                <li>오사카 난바 호텔 추천, 위치 좋아서 만족한 숙소 후기</li>
                <li>제주 애월 감성숙소 2박 후기, 커플여행 숙소 추천</li>
                <li>후쿠오카 3박 4일 숙소 후기, 가성비 호텔 찾는다면</li>
                <li>부산 해운대 오션뷰 호텔 후기, 친구랑 가기 좋았던 숙소</li>
                <li>도쿄 신주쿠 호텔 후기, 지하철 가까운 숙소 추천</li>
              </ol>
            </div>
          </div>

          <div class="section">
            <p class="section-label">[본문 내용]</p>
            <div class="desc-box">
              <ul>
                <li>서론(선택 이유): 왜 이 숙소를 예약했는지</li>
                <li>본론(상세 후기): 위치, 청결, 가격, 장점/아쉬운 점</li>
                <li>결론(총평): 어떤 사람에게 추천하는지</li>
              </ul>
            </div>
          </div>

          <div class="section">
            <p class="section-label">[참고사항]</p>
            <div class="desc-box">
              <ul>
                <li>처음 숙소 링크를 만든다면 아고다를 추천드려요.</li>
                <li>링크는 1번보다 2~3번 넣는 것을 권장해요.</li>
              </ul>
            </div>
          </div>

          <div class="button-wrap">
            <a href="#" class="btn">예시 바로가기</a>
          </div>
        </div>
      </details>

      <details class="card">
        <summary>
          <div class="summary-left">
            <div class="emoji">🛒</div>
            <div class="card-title">최근 구매한 물건 후기 쓰기</div>
          </div>
          <div class="arrow">⌄</div>
        </summary>

        <div class="card-body">
          <div class="section">
            <p class="section-label">[제목 예시]</p>
            <div class="desc-box">
              <ol>
                <li>원룸 제습기 건조기 LG 위닉스 VS 넥스코 미니제습기</li>
                <li>여름맞이 스트레이트 체형 수영복 고르기 후보 추천</li>
                <li>신생아부터 쓰는 브라운 체온계, 밤에 열 체크 편한 체온계 후기</li>
                <li>자취생 필수템 가성비 좋은 롤팩 매트리스 데코라인 실루나</li>
                <li>스타우브 솥밥 냄비 꼬꼬데 20 원형 주물냄비 3개월 사용 후기</li>
              </ol>
            </div>
          </div>

          <div class="section">
            <p class="section-label">[본문 내용]</p>
            <div class="desc-box">
              <ul>
                <li>서론(선택 이유): 왜 이 브랜드, 이 상품을 구매하게 되었는지</li>
                <li>본론(상세 후기): 실제 사용 후기, 장점/아쉬운 점, 가격</li>
                <li>결론(총평/추천 유형): 누구에게 추천하고 싶은지</li>
              </ul>
            </div>
          </div>

          <div class="section">
            <p class="section-label">[참고사항]</p>
            <div class="desc-box">
              <ul>
                <li>처음 상품 링크를 만든다면 오늘의집, 쿠팡 같은 익숙한 프로그램부터 시작해보세요.</li>
                <li>링크는 1번보다 2~3번 넣는 것을 권장해요.</li>
              </ul>
            </div>
          </div>

          <div class="button-wrap">
            <a href="#" class="btn">예시 바로가기</a>
          </div>
        </div>
      </details>
    </section>
  </main>
</body>
</html>
