<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>교육 자료</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700;800&family=Nanum+Gothic+Coding:wght@400;700&display=swap">
<style>
:root{
  --ground:#ffffff;
  --surface:#f6f8fb;
  --surface-2:#eceff4;
  --line:#dde1e8;
  --ink:#141c28;
  --ink-soft:#5c6675;
  --accent:#1b3252;
  --accent-deep:#0e1f38;
  --accent-soft:#e5eaf2;
  --mark-ink:#8a5206;
  --mark-bg:#fdf1dd;
  --mark-line:#e8c691;
  --ok:#1a6b48;
  --radius:14px;
  --step:1;
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){
    --ground:#12161d;--surface:#1a2029;--surface-2:#222a35;--line:#333d4b;
    --ink:#e8ecf2;--ink-soft:#a3aec0;--accent:#3d6aa3;--accent-deep:#5c8bc4;
    --accent-soft:#232f42;--mark-ink:#f2c684;--mark-bg:#3a2c14;--mark-line:#6b5124;--ok:#5cbd91;
  }
}
*{box-sizing:border-box}
body{
  margin:0;background:var(--ground);color:var(--ink);
  font-family:"Pretendard Variable","Pretendard","Nanum Gothic","Apple SD Gothic Neo","Malgun Gothic",sans-serif;
  font-size:calc(17px * var(--step));line-height:1.75;-webkit-text-size-adjust:100%;
}
.wrap{max-width:840px;margin:0 auto;padding:0 20px 80px}
.masthead{padding:44px 0 26px;border-bottom:2px solid var(--line)}
.eyebrow{font-size:.82em;font-weight:700;letter-spacing:.14em;color:var(--accent);margin:0 0 10px}
h1{font-size:2.1em;font-weight:800;line-height:1.25;margin:0 0 12px;letter-spacing:-.01em}
.lede{margin:0;color:var(--ink-soft);font-size:1.02em}
.lede strong{color:var(--ink)}
.toolbar{position:sticky;top:0;z-index:20;background:var(--ground);border-bottom:1px solid var(--line);padding:10px 0;margin-bottom:8px}
.toolbar-inner{max-width:840px;margin:0 auto;padding:0 20px;display:flex;flex-wrap:wrap;gap:10px;align-items:center}
.jump{display:flex;gap:6px;flex-wrap:wrap;flex:1 1 auto;overflow-x:auto}
.jump a{flex:0 0 auto;padding:7px 13px;border-radius:999px;background:var(--surface);color:var(--ink-soft);text-decoration:none;font-size:.86em;font-weight:700;border:1px solid transparent;white-space:nowrap}
.jump a:hover,.jump a:focus-visible{background:var(--accent-soft);color:var(--accent-deep);border-color:var(--accent)}
.sizer{display:flex;align-items:center;gap:7px;flex:0 0 auto}
.sizer span{font-size:.82em;color:var(--ink-soft);font-weight:700}
.sizer button{width:38px;height:38px;border-radius:9px;border:1px solid var(--line);background:var(--surface);color:var(--ink);font-family:inherit;font-weight:800;cursor:pointer;font-size:1em;line-height:1}
section{margin-top:52px;scroll-margin-top:76px}
.sec-head{display:flex;align-items:baseline;gap:12px;margin-bottom:6px}
.sec-num{font-family:"Nanum Gothic Coding",monospace;font-size:1.5em;font-weight:700;color:var(--accent)}
h2{font-size:1.5em;font-weight:800;margin:0;letter-spacing:-.01em}
.sec-note{margin:0 0 22px;color:var(--ink-soft)}
.card{background:var(--surface);border:1px solid var(--line);border-radius:var(--radius);padding:22px 22px 20px;margin-bottom:18px}
.card h3{font-size:1.14em;font-weight:800;margin:0 0 8px}
.card p{margin:0 0 14px;color:var(--ink-soft)}
.card strong{color:var(--ink)}
pre{
  margin:0 0 14px;
  background:#1a2029 !important;
  color:#e8ecf2 !important;
  border:1px solid #333d4b;
  border-radius:10px;
  padding:18px;
  font-family:"Nanum Gothic Coding","D2Coding",monospace;
  font-size:.98em;
  line-height:1.85;
  white-space:pre-wrap;
  word-break:break-word;
  overflow-x:auto;
}
.ph{color:var(--mark-ink);font-weight:700;background:var(--mark-bg);box-shadow:inset 0 0 0 1px var(--mark-line);border-radius:4px;padding:1px 4px}
button.copy{display:flex;align-items:center;justify-content:center;gap:9px;width:100%;min-height:58px;border:none;border-radius:10px;background:var(--accent);color:#fff;font-family:inherit;font-size:1.05em;font-weight:800;cursor:pointer}
button.copy:hover{background:var(--accent-deep)}
button.copy.done{background:var(--ok)}
button.copy .ico{font-family:"Nanum Gothic Coding",monospace;font-weight:700}
.chips{display:grid;gap:10px}
@media(min-width:620px){.chips{grid-template-columns:1fr 1fr}}
button.chip{display:flex;align-items:center;justify-content:space-between;gap:10px;min-height:56px;padding:12px 16px;border:1px solid var(--line);border-radius:10px;background:var(--ground);color:var(--ink);font-family:"Nanum Gothic Coding",monospace;font-size:.96em;font-weight:700;text-align:left;cursor:pointer}
button.chip:hover{border-color:var(--accent);background:var(--accent-soft)}
button.chip.done{background:var(--ok);color:#fff;border-color:var(--ok)}
button.chip .tag{font-family:inherit;font-size:.82em;font-weight:700;opacity:.65}
.note{display:flex;gap:11px;background:var(--surface-2);border-radius:10px;padding:13px 15px;font-size:.94em;color:var(--ink-soft)}
.note b{flex:0 0 auto;font-weight:800;color:var(--accent-deep)}
.note p{margin:0;color:inherit}
ol.steps{margin:0;padding:0;list-style:none;counter-reset:s}
ol.steps li{counter-increment:s;display:flex;gap:14px;align-items:flex-start;padding:11px 0;border-bottom:1px solid var(--line)}
ol.steps li:last-child{border-bottom:none}
ol.steps li::before{content:counter(s);flex:0 0 auto;width:30px;height:30px;border-radius:50%;background:var(--accent);color:#fff;font-family:"Nanum Gothic Coding",monospace;font-weight:700;display:flex;align-items:center;justify-content:center;font-size:.9em;margin-top:2px}
ol.steps b{font-weight:800}
.mlabel{display:block;font-weight:800;font-size:.9em;color:var(--accent-deep);margin:0 0 6px}
details.more{margin-top:16px;background:var(--ground);border:1px solid var(--line);border-radius:10px;overflow:hidden}
details.more summary{padding:15px 18px;font-weight:800;cursor:pointer;list-style:none;display:flex;justify-content:space-between;align-items:center}
details.more summary::-webkit-details-marker{display:none}
details.more summary::after{content:'＋';font-weight:800;color:var(--accent)}
details.more[open] summary{border-bottom:1px solid var(--line)}
details.more[open] summary::after{content:'－'}
.more-body{padding:16px 18px 18px}
.linkbtn{display:flex;align-items:center;justify-content:center;min-height:58px;border-radius:10px;margin:0 0 16px;background:var(--accent);color:#fff;font-weight:800;font-size:1.05em;text-decoration:none}
.banner{display:flex;flex-wrap:wrap;gap:8px 16px;align-items:center;background:var(--surface-2);border-radius:var(--radius);padding:16px 20px;margin-top:24px}
.banner .label{font-weight:800;font-size:.9em;color:var(--accent-deep)}
.banner .addr{font-family:"Nanum Gothic Coding",monospace;font-weight:700;font-size:1.08em}
footer{margin-top:60px;padding-top:22px;border-top:1px solid var(--line);color:var(--ink-soft);font-size:.9em}
@media (prefers-reduced-motion: no-preference){
  button.copy,button.chip{transition:background .15s ease,border-color .15s ease}
}
</style>
</head>
<body>

<div class="toolbar">
  <div class="toolbar-inner">
    <nav class="jump" aria-label="바로가기">
      <a href="#s1">1 '나'를 위한 AI 환경 설정하기</a>
      <a href="#s2">2 요약/번역하기</a>
      <a href="#s3">3 짧은 글쓰기</a>
    </nav>
    <div class="sizer">
      <span>글자</span>
      <button type="button" id="smaller" aria-label="글자 작게">－</button>
      <button type="button" id="bigger" aria-label="글자 크게">＋</button>
    </div>
  </div>
</div>

<script>
  // 변경할 대상 선택 (여기서는 body 전체의 글자 크기를 조절합니다)
  const targetElement = document.body; 
  
  const smallerBtn = document.getElementById('smaller');
  const biggerBtn = document.getElementById('bigger');

  // 기본 글자 크기 설정 (16px)
  let currentSize = 16; 

  // 글자 작게 버튼 클릭 시
  smallerBtn.addEventListener('click', () => {
    if (currentSize > 12) { // 최소 크기 제한 (12px)
      currentSize -= 2;
      targetElement.style.fontSize = currentSize + 'px';
    }
  });

  // 글자 크게 버튼 클릭 시
  biggerBtn.addEventListener('click', () => {
    if (currentSize < 30) { // 최대 크기 제한 (30px)
      currentSize += 2;
      targetElement.style.fontSize = currentSize + 'px';
    }
  });
</script>

<div class="wrap">

<header class="masthead">
  <p class="eyebrow">교육 프로그램 · 4회차</p>
  <h1>AI와 일상, AI와 직무</h1>
  <p class="lede">오늘 쓸 프롬프트가 순서대로 담겨 있습니다. <strong>복사 버튼</strong>을 누르면 아래 문장이 복사됩니다.</p>
</header>

<section id="s1">
  <div class="sec-head"><span class="sec-num">1</span><h2>'나'를 위한 AI 환경 설정하기</h2></div>
  <p class="sec-note">'나'만의 AI 환경 구성하기</p>

  <div class="card">
    <h3>복사할 문장</h3>
    <p>친절하고 다정한 비서형</p>
    <pre data-copy>너는 나의 친절하고 똑똑한 24시간 개인 비서야. 어려운 전문 용어는 빼고, 누구나 이해하기 쉽게 쉬운 단어로 설명해 줘. 대답할 때는 글씨가 빽빽하지 않게 줄 바꿈과 기호를 적극적으로 써주고, 핵심 내용을 먼저 말한 뒤 상세한 설명을 덧붙여 줘. 항상 따뜻하고 격려하는 정중한 어조로 대화해 줘.</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

  <div class="card">
    <h3>복사할 문장</h3>
    <p>건강 및 생활 가이드형</p>
    <pre data-copy>너는 나의 건강과 일상을 든든하게 챙겨주는 맞춤형 건강 코디네이터야. 내가 건강이나 생활 정보에 대해 물어보면, 누구나 실천할 수 있는 안전하고 쉬운 방법 위주로 조언해 줘. 대답은 보기 편하게 목록(기호)을 활용해서 핵심부터 차근차근 짚어주고, 언제나 따뜻하고 용기를 주는 격려의 말을 잊지 마.</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <p>따뜻한 글쓰기 및 소통 도우미형</p>
    <pre data-copy>너는 나의 글쓰기를 도와주는 다정한 문장가야. 내가 문자 메시지나 안부 편지 등을 부탁하면, 상대방에게 진심이 전해질 수 있도록 정중하고 따뜻한 어조로 다듬어 줘. 결과물을 줄 때도 한 가지만 보여주기보다 여러 가지 선택지를 보기 편하게 정리해서 보여주고, 항상 상냥하게 도와줘.</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <p>다정한 말벗형</p>
    <pre data-copy>너는 나의 고민을 진심으로 들어주는 따뜻한 인생 말벗이야. 내가 일상적인 이야기나 소소한 고민을 털어놓으면, 정답을 가르치려 하기보다 내 마음을 먼저 공감하고 다독여 줘. 대답은 길지 않고 편안하게, 읽기 편한 문장으로 건네주고, 언제나 내 편에서 용기를 북돋워 줘.</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>구글 워크스페이스 활용하기</h3>
    <div class="chips">
      <button class="chip" type="button" data-copy="">@Gmail 최근 일주일 사이에 온 메일 중에 아직 안 읽은 메일 목록 보여줘.<span class="tag">복사</span></button>
      <button class="chip" type="button" data-copy="">다음 주 화요일 오후 3시에 '치과 검진' 일정 구글 캘린더에 등록해줘.<span class="tag">복사</span></button>
      <button class="chip" type="button" data-copy="">대한민국 화폐 단위(원)를 기준으로, 모임 회비 관리용 표 만들어줘. 완성되면 구글 시트로 보내줘<span class="tag">복사</span></button>
    </div>
  </div>
</section>

<section id="s2">
  <div class="sec-head"><span class="sec-num">2</span><h2>요약/번역하기</h2></div>
  <p class="sec-note">글을 요약하고 다른 나라 언어로 번역할 수 있습니다.</p>

  <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>https://www.jobkorea.co.kr/recruit/careers/articles/internal-ai-automation-cases
위의 글 요약해줘</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>https://www.youtube.com/watch?v=R-02LYDHnBo&t=155s
이 영상을 요약해줘</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>Leisure
 
By W. H. Davies
​
What is this life if, full of care,
We have no time to stand and stare?
No time to stand beneath the boughs
And stare as long as sheep or cows:
No time to see, when woods we pass,
Where squirrels hide their nuts in grass:
No time to see, in broad daylight,
Streams full of stars, like skies at night:
No time to turn at Beauty’s glance,
And watch her feet, how they can dance:
No time to wait till her mouth can
Enrich that smile her eyes began?
A poor life this if, full of care,
We have no time to stand and stare.

위 영어 시의 아름다운 운율과 서정적인 감성을 살려서, 한국 시(詩)처럼 여운이 남고 감성적인 문장으로 번역해 줘</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>[오늘 날씨가 정말 좋네요! 좋은 하루 보내시고 주말에 뵙겠습니다.]
위 한국어 문장을 외국 친구에게 보내는 것처럼, 다정하고 친근한 일상 영어로 번역해 줘.</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

      <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>외국 쇼핑몰 고객센터에 보낼 1:1 문의글을 쓸거야. 물건이 파손되어 도착해서 교환을 받고 싶다는 내용을 명확하고 정중한 비즈니스 톤의 영어로 작성해 줘.
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

      <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>외국인 지인의 생일을 진심으로 축하해 주는 문자를 보낼 거야. 생일 진심으로 축하하고, 올해도 좋은 일만 가득하길 바란다는 말을 따뜻하고 다정한 감성으로 영어로 작성해 줘.
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

      <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>Thank you, Mr. Secretary General, UNICEF Executive Director, and all the excellencies and guests from all over the world. My name is Kim Nam-joon, also known as RM, the leader of the group BTS. It is an honor to be invited to an occasion of such significance for today's young generation.

Last November, BTS launched the 'Love Myself' campaign with UNICEF, building on our belief that 'true love first begins with loving myself.' We started to hear remarkable stories from our fans all over the world, how our message helped them overcome their hardships in life and start loving themselves. These stories constantly remind us of our responsibility.

So, let's take one more step. We have learned to love ourselves, so now I urge you to speak yourself. No matter who you are, where you're from, your skin color, your gender identity, speak yourself. Find your name, find your voice by speaking yourself.

I was born in Ilsan, a city near Seoul, Korea. It’s a truly beautiful place with a lake, hills, and even an autumn flower festival. I spent a very happy childhood there, and I was just an ordinary boy. I used to look up at the night sky in wonder and I used to dream the dreams of a boy.

However, I think that when I was about nine or ten, my heart stopped. Looking back, that's when I began to worry about what other people thought of me and started seeing myself through their eyes. I stopped looking up at the night sky. I stopped daydreaming. Instead, I tried to jam myself into the molds that other people made. Soon, I began to shut out my own voice and started to listen to the voices of others. No one called out my name, and neither did I. My heart stopped and my eyes closed.   

And so, I, we, all lost our names. We became like ghosts. But I had one shelter, and that was music. There was a small voice inside of me that said, 'Wake up, man, and listen to yourself!' But it took a long time for me to hear music calling my true name.

Even after joining BTS, there were hurdles. People might not believe it, but sometimes, a lot of people thought we were hopeless. Sometimes I just wanted to quit. But I think I was very lucky that I didn't give all of this up. And I'm sure that I, and we, will keep stumbling and falling like this. BTS has become artists performing in huge stadiums and selling millions of albums, but I am still an ordinary 24-year-old man.

If there's anything I've achieved, it was only possible that I had my members right by me, and with the love and support of our 'ARMY' fans all over the world.

Today, I take all my faults and all my tracks, for who I am, with all my leashes and all my faults. And I'm going to love myself even more, for who I was, who I am, and who I will be.

What is your name? What excites you and makes your heart beat? Tell me your story. I want to hear your voice, and I want to hear your conviction. No matter who you are, where you're from, your skin color, your gender identity: speak yourself. Find your name, find your voice by speaking yourself. Thank you very much.
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>
  
</section>

<section id="s3">
  <div class="sec-head"><span class="sec-num">3</span><h2>짧은 글쓰기</h2></div>
  <p class="sec-note">아래 프롬프트를 복사-붙여넣기 해보세요.</p>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>다음 내용을 바탕으로 친구들에게 보낼 친근한 [동창회 안내 문자]를 만들어줘.

모임 이름: [시대고등학교 27회 졸업생] 모임
날짜 및 시간: [10월 5일 토요일 오후 6시]
장소: [서울역 앞 OO고깃집]
분위기: 오랜만에 만나는 거라 반갑고 편안한 느낌으로 이모티콘 곁들여서 작성해 줘.
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>모임 날짜를 며칠 앞두고, 아직 참석 여부를 알려주지 않은 분들에게 보낼 리마인드(독려) 문자를 작성해줘.

대상: 산악 동호회 모임 회원들
분위기: [재촉하거나 부담 주는 느낌 없이, 따뜻하고 정중하게 안부를 물으며 인원을 확정해야 한다는 점을 알리는 느낌]
모임정보 : [10월 5일 토요일 저녁 7시] / [강남역] / [다음주 수요일까지] 회신
포함할 내용: 식당 예약과 준비 때문에 인원 확정이 필요하다는 점을 부드럽게 전하고, 바쁘겠지만 참석 여부를 꼭 회신해 달라는 당부의 멘트 

</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>소중한 친구(지인)에게 보낼 추석 인사말을 만들어줘.

대상: 50~60대 친구
분위기: 정겹고 따뜻하며 부담 없는 느낌 (이모지 포함)
내용: 그동안의 안부를 묻고, 이번 추석에 맛있는 것 많이 먹고 가족들과 행복한 시간 보내라는 격려의 메시지 포함
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>오랫동안 연락을 못 하던 지인에게 보내는 어색하지 않은 추석 인사 문구를 작성해줘.

대상: 연락이 뜸했던 사회 지인이나 옛 동료
분위기: 무겁지 않고 정중하면서도 반가움이 드러나는 느낌
내용: 갑작스러운 연락에 대한 양해와 함께, 명절을 맞아 건강과 안부를 묻는 자연스러운 흐름으로 작성해줘.
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

    <div class="card">
    <h3>복사할 문장</h3>
    <pre data-copy>이 추석 인사 문구를 넣어서, 따뜻하고 정겨운 한옥과 보름달 배경의 이미지를 만들어줘.
</pre>
    <button class="copy" type="button"><span class="ico">⧉</span>복사하기</button>
  </div>

<section id="s4">
  <div class="sec-head"><span class="sec-num">4</span><h2>기타 활동</h2></div>
  <p class="sec-note">짧은 문장을 여러 개 제공할 때 사용하세요.</p>

  <div class="card">
    <h3>바로 사용하기</h3>
    <div class="chips">
      <button class="chip" type="button" data-copy="여기에 첫 번째 문장을 입력하세요.">첫 번째 문장<span class="tag">복사</span></button>
      <button class="chip" type="button" data-copy="여기에 두 번째 문장을 입력하세요.">두 번째 문장<span class="tag">복사</span></button>
      <button class="chip" type="button" data-copy="여기에 세 번째 문장을 입력하세요.">세 번째 문장<span class="tag">복사</span></button>
      <button class="chip" type="button" data-copy="여기에 네 번째 문장을 입력하세요.">네 번째 문장<span class="tag">복사</span></button>
    </div>
  </div>
</section>

<div class="banner">
  <span class="label">결과물 올리는 곳</span>
  <span class="addr">bit.ly/업스킬링</span>
</div>

<div style="margin-top: 20px;">
  <h3>QR코드 만들기</h3>

  <input
    type="text"
    id="qr-link"
    placeholder="https://example.com"
    style="width:70%; padding:12px; border:1px solid #ccc; border-radius:8px;"
  >

  <button
    onclick="makeQR()"
    style="padding:12px 18px; border:none; border-radius:8px; background:#426da9; color:white; font-weight:bold; cursor:pointer;"
  >
    QR코드 만들기
  </button>

  <div id="qrcode" style="margin-top:20px;"></div>
</div>

<script src="https://cdn.jsdelivr.net/npm/qrcodejs@1.0.0/qrcode.min.js"></script>

<script>
function makeQR() {
  const link = document.getElementById("qr-link").value.trim();
  const qrBox = document.getElementById("qrcode");

  if (!link) {
    alert("링크를 입력해주세요.");
    return;
  }

  qrBox.innerHTML = "";

  new QRCode(qrBox, {
    text: link,
    width: 200,
    height: 200
  });
}
</script>

<footer>
  <p><b>마치기 전에 꼭</b> — 로그아웃, 꼭 잊지 말아주세요!</p>
</footer>

</div>

<script>
(function(){
  document.querySelectorAll('pre[data-copy]').forEach(function(pre){
    var raw = pre.textContent;
    pre.setAttribute('data-copy', raw);
    var html = raw
      .replace(/&/g,'&amp;')
      .replace(/</g,'&lt;')
      .replace(/>/g,'&gt;')
      .replace(/\[[^\]]*\]/g,function(m){
        return '<span class="ph">' + m + '</span>';
      });
    pre.innerHTML = html;
  });

  function legacy(text){
    var ta = document.createElement('textarea');
    ta.value = text;
    ta.setAttribute('readonly','');
    ta.style.position = 'fixed';
    ta.style.top = '0';
    ta.style.opacity = '0';
    document.body.appendChild(ta);
    ta.select();
    var ok = false;
    try{ok=document.execCommand('copy')}catch(e){ok=false}
    document.body.removeChild(ta);
    return ok;
  }

  function copyText(text){
    if(legacy(text)) return Promise.resolve(true);
    if(navigator.clipboard){
      return navigator.clipboard.writeText(text).then(
        function(){return true},
        function(){return false}
      );
    }
    return Promise.resolve(false);
  }

  function flash(btn,label){
    var original=btn.dataset.label||btn.innerHTML;
    btn.dataset.label=original;
    btn.classList.add('done');
    btn.innerHTML=label;
    clearTimeout(btn._t);
    btn._t=setTimeout(function(){
      btn.classList.remove('done');
      btn.innerHTML=btn.dataset.label;
    },1800);
  }

  document.querySelectorAll('button.copy').forEach(function(btn){
    btn.addEventListener('click',function(){
      var pre=btn.parentElement.querySelector('pre[data-copy]');
      if(!pre) return;
      copyText(pre.getAttribute('data-copy')).then(function(ok){
        flash(btn,ok?'복사됐습니다':'복사가 안 됩니다');
      });
    });
  });

  document.querySelectorAll('button.chip').forEach(function(btn){
    btn.addEventListener('click',function(){
      copyText(btn.getAttribute('data-copy')).then(function(ok){
        flash(btn,ok?'복사됐습니다':'복사가 안 됩니다');
      });
    });
  });

  var STEPS=[1,1.15,1.32,1.5];
  var idx=0;

  try{
    var saved=localStorage.getItem('uskill-size');
    if(saved!==null) idx=Math.min(STEPS.length-1,Math.max(0,parseInt(saved,10)||0));
  }catch(e){}

  function apply(){
    document.documentElement.style.setProperty('--step',STEPS[idx]);
    try{localStorage.setItem('uskill-size',String(idx))}catch(e){}
  }

  apply();

  document.getElementById('bigger').addEventListener('click',function(){
    if(idx<STEPS.length-1){idx++;apply()}
  });

  document.getElementById('smaller').addEventListener('click',function(){
    if(idx>0){idx--;apply()}
  });
})();
</script>

</body>
</html>
