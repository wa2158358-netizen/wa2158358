# wa2158358
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Noto Sans KR', sans-serif;
      line-height: 1.6;
      background-color: #f4f4f4;
      color: #333;
      padding: 20px;
    }

    header {
      text-align: center;
      margin-bottom: 30px;
    }

    header h1 {
      font-size: 2rem;
      color: #222;
    }

    .container {
      display: grid;
      gap: 20px;
    }

    section {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }

    section h2 {
      margin-bottom: 10px;
      color: #0056a1;
    }

    /* 모바일 (기본) */
    @media (max-width: 599px) {
      .container {
        grid-template-columns: 1fr;
      }
      header h1 { font-size: 1.6rem; }
    }

    /* 태블릿 */
    @media (min-width: 600px) and (max-width: 1023px) {
      .container {
        grid-template-columns: 1fr 1fr;
        grid-template-areas:
          "about projects"
          "education another"
          "strengths strengths";
      }
      #about { grid-area: about; }
      #education { grid-area: education; }
      #another { grid-area: another; }
      #projects { grid-area: projects; }
      #strengths { grid-area: strengths; }
    }

    /* 데스크톱 */
    @media (min-width: 1024px) {
      .container {
        grid-template-columns: 1.5fr 1fr 1fr;
        grid-template-areas:
          "about education strengths"
          "projects another strengths";
      }
      #about { grid-area: about; }
      #education { grid-area: education; }
      #another { grid-area: another; }
      #projects { grid-area: projects; }
      #strengths { grid-area: strengths; }
    }
  </style>
</head>
<body>
  <header>
    <h1>My Portfolio</h1>
    <p>CAD 디자이너 & 행정 실무자</p>
  </header>

  <div class="container">
    <section id="about">
      <h2>About Me</h2>
      <p>안녕하세요! 저는 남부대학교 방사선학과를 졸업하고 CAD 관심있어서 sbs아카데미 학원에서 한달 배움으로 조금 더 CAD에 관심이 생겨서 </p>
    </section>

    <section id="education">
      <h2>Education</h2>
      <ul>
        <li>CAD 아카데미 수료 (2024)</li>        
      </ul>
    </section>

    <section id="another">
      <h2>Another Experience</h2>
      <p>건설 현장 안전관리 업무 경험이 있습니다.</p>
    </section>

    <section id="strengths">
      <h2>Strengths</h2>
      <ul>
        <li>정확한 도면 작성 능력</li>
        <li>문서 정리 및 일정 관리</li>
        <li>팀워크와 커뮤니케이션 능력</li>
      </ul>
    </section>
  </div>
</body>
</html>

