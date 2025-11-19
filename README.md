<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>커스텀 폰트 테스트</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <nav class="menu-bar">
    <label>폰트 선택:
      <select id="font-select">
        <option value="Londerground">LDN Round</option>
        <option value="MAN HEX">MAN HEX</option>
        <option value="EDISerif">EDI Serif</option>
      </select>
    </label>
    <label>정렬:</label>
    <span id="align-controls" class="align-controls" role="toolbar" aria-label="정렬 선택">
        <button type="button" class="align-btn active" data-align="left" title="왼쪽 정렬" aria-label="왼쪽 정렬">
          <!-- left align icon -->
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <rect x="3" y="5" width="14" height="2"></rect>
            <rect x="3" y="10" width="20" height="2"></rect>
            <rect x="3" y="15" width="14" height="2"></rect>
          </svg>
        </button>
        <button type="button" class="align-btn" data-align="center" title="가운데 정렬" aria-label="가운데 정렬">
          <!-- center align icon -->
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <rect x="5" y="5" width="14" height="2"></rect>
            <rect x="3" y="10" width="18" height="2"></rect>
            <rect x="5" y="15" width="14" height="2"></rect>
          </svg>
        </button>
        <button type="button" class="align-btn" data-align="right" title="오른쪽 정렬" aria-label="오른쪽 정렬">
          <!-- right align icon -->
          <svg viewBox="0 0 24 24" aria-hidden="true" focusable="false">
            <rect x="7" y="5" width="14" height="2"></rect>
            <rect x="3" y="10" width="20" height="2"></rect>
            <rect x="7" y="15" width="14" height="2"></rect>
          </svg>
        </button>
        <!-- Justify button removed per user request -->
      </span>
    <label>자간:
      <input type="range" id="letter-spacing" min="-10" max="20" value="0"> <span id="letter-spacing-value">0</span>px
    </label>
    <label>행간:
      <input type="range" id="line-height" min="-10" max="40" value="20"> <span id="line-height-value">2.0</span>
    </label>
    <label>폰트 크기:
      <input type="range" id="font-size" min="10" max="60" value="24"> <span id="font-size-value">24</span>px
    </label>
    <label>색상:
      <input type="color" id="font-color" value="#222222">
    </label>
  </nav>

    <main>
    <div id="demo-text" class="editable-text" contenteditable="true" data-placeholder="여기에 글을 입력하면 선택한 폰트로 입력됩니다.
해당 폰트는 영어 전용 폰트로, 영어만 입력이 가능합니다.
입력이 되지 않을 경우, 한/영 전환 상태를 확인해주시기 바랍니다.
폰트, 정렬, 자간, 행간, 크기, 색상 등을 자유롭게 변경하며 사용해보시기 바랍니다." data-empty="true"></div>
  </main>
  
  <div class="site-tagline">See it, Type it, Sorted.</div>

  <script src="main.js"></script>
</body>
</html>
