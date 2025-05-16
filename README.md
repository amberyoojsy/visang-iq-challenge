<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no" />
  <title>Visang IQ Challenge</title>

  <!-- Pretendard 로드를 위한 Preconnect -->
  <link rel="preconnect" href="https://unpkg.com" />

  <!-- Pretendard CSS via unpkg -->
  <link
    rel="stylesheet"
    href="https://unpkg.com/pretendard@1.3.6/dist/web/static/pretendard.css"
  />

  <style>
    /* ─────────────────────────────────────────
       아래는 기존에 쓰시던 CSS를 그대로 붙여주세요
       ───────────────────────────────────────── */
    body {
      font-family: 'Pretendard', sans-serif;
      padding: 20px;
      background: url('https://i.imgur.com/ggotSIY.jpeg') no-repeat center center / cover, #e0f7fa;
      color: #333;
    }
    h1 {
      max-width: 700px;
      margin: 0 auto 20px;
      text-align: center;
      font-size: 4em;
      color: #fff;
      text-shadow:
        -4px -4px 0 #333,
        4px -4px 0 #333,
        -4px 4px 0 #333,
        4px 4px 0 #333;
    }
    .intro {
      max-width: 700px;
      margin: 0 auto 30px;
      background: linear-gradient(135deg, #ffffff 0%, #e0f7fa 100%);
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      position: relative;
    }
    .intro::before {
      content: "📝";
      position: absolute;
      top: -16px;
      left: 16px;
      font-size: 28px;
    }
    .intro p { margin: 10px 0; line-height: 1.5; font-weight: 600; }
    /* ... 이하 생략하지 말고 기존 CSS 전부 붙이기 ... */
  </style>
</head>
<body>
  <h1>Visang IQ Challenge</h1>
  <div class="intro">
    <p>CP님들께서 비상을 더 즐겁고 흥미롭게 알아가실 수 있도록</p>
    <p>비상의 비전, 역사, 그리고 사옥에 대한 퀴즈,<br />바로 🌟 <strong>VISANG IQ (Identity Quiz)</strong> 🌟를 준비했습니다!</p>
    <p>💡 챌린지를 통과하신 후에는 페들렛에 궁금한 점이나, 퀴즈를 통해 생긴 질문들을 자유롭게 남겨주세요.</p>
    <p>비상의 뿌리와 비전을 자연스럽게 이해하며 자부심을 느끼는 시간이 되시길 바랍니다. 감사합니다. 💛</p>
  </div>

  <!-- 1) action·target·숨김필드 추가 -->
  <form
    id="quizForm"
    action="https://script.google.com/macros/s/AKfycbyBm9ochv6aOdQufS2EL9YOfs8yMwM5n5ZIyTy907OBoDS-4olCNBiqpNO8RI1UL_4P/exec"
    method="post"
    target="submitFrame"
  >
    <!-- 사용자 정보 -->
    <div class="question">
      <h3>이름을 입력해 주세요!<span class="required-note">*</span></h3>
      <input type="text" name="userName" placeholder="이름을 입력해 주세요!" required />
    </div>
    <div class="question">
      <h3>사번을 입력해 주세요!<span class="required-note">*</span></h3>
      <input type="text" name="employeeId" placeholder="사번을 입력해 주세요!" required />
    </div>

    <!-- 1–14 객관식 -->
    <div class="question"><h3 data-question="1">2023년 비상교육의 경영 방침은 무엇이었나요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q1" value="a" /> 콘텐츠 다양화</label>
      <label><input type="radio" name="q1" value="b" /> 디지털 전환</label>
      <label><input type="radio" name="q1" value="c" /> 글로벌 진출</label>
      <label><input type="radio" name="q1" value="d" /> 조직 축소</label>
    </div>
    <!-- 나머지 객관식에도 동일하게 첫 input에 required, h3 뒤에 * 표시 -->
    <!-- ... q2 ~ q14 생략하지 않고 모두 포함 ... -->
    <div class="question"><h3 data-question="2">2024년~2025년의 경영방침은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q2" value="a" /> 유아 교육 제품 확대</label>
      <label><input type="radio" name="q2" value="b" /> 컴퍼니 간 연계 강화</label>
      <label><input type="radio" name="q2" value="c" /> 해외 영업 확장</label>
      <label><input type="radio" name="q2" value="d" /> 교과서 디자인 개선</label>
    </div>
    <div class="question"><h3 data-question="3">비상교육의 디지털 전환을 위한 업무 방식 중 도입되지 않은 것은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q3" value="a" /> 전사 통(회의)시간 단축</label>
      <label><input type="radio" name="q3" value="b" /> M365 프로그램 도입</label>
      <label><input type="radio" name="q3" value="c" /> 페이퍼리스 정책</label>
      <label><input type="radio" name="q3" value="d" /> 하이브리드 근무 시행</label>
    </div>
    <div class="question"><h3 data-question="4">우리의 믿음이 선포된 VIVA Summit Meeting은 언제 진행되었나요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q4" value="a" /> 2018년 6월 15일</label>
      <label><input type="radio" name="q4" value="b" /> 2017년 10월 20일</label>
      <label><input type="radio" name="q4" value="c" /> 2018년 10월 20일</label>
      <label><input type="radio" name="q4" value="d" /> 2019년 6월 15일</label>
    </div>
    <div class="question"><h3 data-question="5">'온리원'은 어떤 학습 개념에 기반한 프로그램인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q5" value="a" /> 감정 조절</label>
      <label><input type="radio" name="q5" value="b" /> 암기 훈련</label>
      <label><input type="radio" name="q5" value="c" /> 메타인지</label>
      <label><input type="radio" name="q5" value="d" /> 프로젝트 수업</label>
    </div>
    <div class="question"><h3 data-question="6">‘컴퍼니 간 연계와 융합 틀’을 마련하기 위해 비상이 계속 추진해야 할 과업은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q6" value="a" /> 각 컴퍼니별 분리 운영</label>
      <label><input type="radio" name="q6" value="b" /> 전사 데이터 정렬·통합</label>
      <label><input type="radio" name="q6" value="c" /> 신규 HR 평가 제도 도입</label>
      <label><input type="radio" name="q6" value="d" /> 해외 법인 설립</label>
    </div>
    <div class="question"><h3 data-question="7">디지털 교과서의 세 가지 핵심 조건으로 올바르게 짝지어진 것은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q7" value="a" /> 교과 과정 디지털화–학습 과정 데이터화–수업 과정 플랫폼화</label>
      <label><input type="radio" name="q7" value="b" /> 평가 강화–콘텐츠 다양화–교육청 연계</label>
      <label><input type="radio" name="q7" value="c" /> 메타인지–피드백–진도관리</label>
      <label><input type="radio" name="q7" value="d" /> 제작–연수–고도화</label>
    </div>
    <div class="question"><h3 data-question="8">ICS(Interactive Class System)’가 구현하고자 하는 핵심 요소는 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q8" value="a" /> 일방향 강의</label>
      <label><input type="radio" name="q8" value="b" /> 교사 중심 강의</label>
      <label><input type="radio" name="q8" value="c" /> 평가 시험</label>
      <label><input type="radio" name="q8" value="d" /> 양방향 소통 및 데이터 피드백</label>
    </div>
    <div class="question"><h3 data-question="9">에듀테크 제품이 학교에 본격 도입될 때, 우리가 가장 지켜야 할 교육적 가치는 무엇이라 생각하나요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q9" value="a" /> 학습자 중심</label>
      <label><input type="radio" name="q9" value="b" /> 기술의 재미</label>
      <label><input type="radio" name="q9" value="c" /> 성적 향상만</label>
      <label><input type="radio" name="q9" value="d" /> 빠른 확장</label>
    </div>
    <div class="question"><h3 data-question="10">AI 디지털 교과서 개발의 주된 목표 중 하나는 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q10" value="a" /> 교사 수 증가</label>
      <label><input type="radio" name="q10" value="b" /> 디지털화 및 메타인지 향상</label>
      <label><input type="radio" name="q10" value="c" /> 공간 확장</label>
      <label><input type="radio" name="q10" value="d" /> 내용 물리적 교환</label>
    </div>
    <div class="question"><h3 data-question="11">비상교육 창립 20주년을 기념하여 도입한 제도 중, 새로운 조직 문화를 반영하기 위해 변경된 부분은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q11" value="a" /> 새로운 CI 도입</label>
      <label><input type="radio" name="q11" value="b" /> 비대면 전환</label>
      <label><input type="radio" name="q11" value="c" /> 호칭을 “CP”로 통일</label>
      <label><input type="radio" name="q11" value="d" /> 근무 시간 단축</label>
    </div>
    <div class="question"><h3 data-question="12">'밸류업' 시스템의 주요 목적은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q12" value="a" /> 경쟁 강화</label>
      <label><input type="radio" name="q12" value="b" /> 평가 정확성</label>
      <label><input type="radio" name="q12" value="c" /> 성장과 의미 증대</label>
      <label><input type="radio" name="q12" value="d" /> 수익 증대</label>
    </div>
    <div class="question"><h3 data-question="13">신사옥의 이름 'ground V'에 포함된 의미가 아닌 것은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q13" value="a" /> Vision</label>
      <label><input type="radio" name="q13" value="b" /> Verb</label>
      <label><input type="radio" name="q13" value="c" /> Variety</label>
      <label><input type="radio" name="q13" value="d" /> Victory</label>
    </div>
    <div class="question"><h3 data-question="14">'ground V' 사옥 건축에서 정형을 탈피한 설계 특징이 아닌 것은 무엇인가요?<span class="required-note">*</span></h3>
      <label><input type="radio" name="q14" value="a" /> 층간 투시</label>
      <label><input type="radio" name="q14" value="b" /> 長 span 구조</label>
      <label><input type="radio" name="q14" value="c" /> 고층 설계</label>
      <label><input type="radio" name="q14" value="d" /> 기둥 최소화</label>
    </div>

    <!-- 15–17 주관식 -->
    <div class="question"><h3 data-question="15">'디지털 전환’이라는 말을 들었을 때 가장 먼저 떠오르는 느낌은 무엇인가요?</h3>
      <textarea name="q15" placeholder="“디지털 전환”이란 말을 들으면, ‘경험이 새롭게 재구성된다’는 느낌이 먼저 들어요!"></textarea>
    </div>
    <div class="question"><h3 data-question="16">2025년의 나, 조직, 회사가 ‘비상’하기 위해 당신이 다짐하는 한 가지는 무엇인가요?</h3>
      <textarea name="q16" placeholder="모두가 함께 배우고 성장할 수 있는 문화를 만들고 싶습니다. 🤝"></textarea>
    </div>
    <div class="question"><h3 data-question="17">양태회 CP님과의 대화를 통해, 새로운 이야기나 생각을 나눌 수 있다는 점에서 기대되는 것이 있다면 자유롭게 적어주세요. 😊</h3>
      <textarea name="q17" placeholder="오랜 경험을 바탕으로 쌓인 CP님의 ‘현장 솔루션’ 이야기를 듣고 싶습니다!🤩"></textarea>
    </div>

    <!-- 숨김 필드 -->
    <input type="hidden" name="score" id="inputScore" />
    <input type="hidden" name="q15" id="inputQ15" />
    <input type="hidden" name="q16" id="inputQ16" />
    <input type="hidden" name="q17" id="inputQ17" />

    <div class="submit-container" style="text-align:center">
      <button type="submit">제출하기</button>
    </div>
  </form>

  <!-- 숨김 iframe -->
  <iframe name="submitFrame" style="display:none;"></iframe>

  <!--팝업-->
  <div class="popup-overlay" id="popup">
    <div class="popup-content" id="popupContent"></div>
  </div>

  <!-- 2) JS: form.submit() 로직 -->
  <script>
  console.log('✅ 스크립트 로드 완료');
  const form = document.getElementById('quizForm');
  console.log('🔍 form 객체:', form);
  if (!form) throw new Error('quizForm을 찾을 수 없습니다.');

  let retryCount = 0;
  const correctAnswers = {
    q1:'b', q2:'b', q3:'a', q4:'b', q5:'c',
    q6:'b', q7:'a', q8:'d', q9:'a', q10:'b',
    q11:'c', q12:'c', q13:'c', q14:'c'
  };

  form.addEventListener('submit', function(e) {
    console.log('🛎️ submit 핸들러 호출됨');
    e.preventDefault();

    // 1) 사용자 정보 & 점수 계산
    const userName   = this.querySelector('input[name="userName"]').value;
    const employeeId = this.querySelector('input[name="employeeId"]').value;
    let score = 0;
    const total = Object.keys(correctAnswers).length;

    // 2) 피드백 초기화
    document.querySelectorAll('.question').forEach(el => {
      el.classList.remove('correct','wrong');
      const old = el.querySelector('.feedback');
      if (old) old.remove();
    });

    // 3) 채점 및 클래스/피드백
    for (const q in correctAnswers) {
      const sel = this.querySelector(`input[name="${q}"]:checked`);
      const container = this.querySelector(`input[name="${q}"]`).closest('.question');
      const fb = document.createElement('span');
      fb.classList.add('feedback');
      if (sel && sel.value === correctAnswers[q]) {
        score++;
        container.classList.add('correct');
        fb.classList.add('correct');
        fb.textContent = '정답!🙆🏻‍♂️';
      } else {
        container.classList.add('wrong');
        fb.classList.add('wrong');
        fb.textContent = '오답!🙅🏻‍♂️';
      }
      container.appendChild(fb);
    }

    // 4) 주관식 값 추출
    const q15 = this.querySelector('textarea[name="q15"]').value;
    const q16 = this.querySelector('textarea[name="q16"]').value;
    const q17 = this.querySelector('textarea[name="q17"]').value;

    // 5) 숨김 필드에 값 채우고 폼 제출
    this.querySelector('#inputScore').value = score;
    this.querySelector('#inputQ15').value   = q15;
    this.querySelector('#inputQ16').value   = q16;
    this.querySelector('#inputQ17').value   = q17;
    
    // → 여기서 폼을 submit 해서 Apps Script로 전송
    this.submit();

    console.log(`제출자: ${userName} (${employeeId}), 점수: ${score}/${total}`);

    // 6) 팝업 띄우기
    const popup = document.getElementById('popup');
    const content = document.getElementById('popupContent');
    content.innerHTML = `<div>수고하셨습니다 🤓 총 ${total}문항 중 ${score}점 획득하셨습니다.</div>`;

    if (score <= 11) {
      retryCount++;
      const div = document.createElement('div');
      div.classList.add('retry-message');
      div.textContent = retryCount < 2
        ? '한 번의 재도전 기회가 있습니다! 🤓'
        : '재도전 기회가 모두 소진되었습니다.';
      content.appendChild(div);
    }

    const btn = document.createElement('button');
    btn.textContent = '확인';
    btn.onclick = () => (popup.style.display = 'none');
    content.appendChild(btn);

    popup.style.display = 'flex';

    // 7) 재도전 2회 소진 시 버튼 제거
    if (retryCount >= 2) {
      document.querySelector('.submit-container')?.remove();
    }
  });
</script>
