<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>온라인 줄넘기 대회 관리 시스템</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
    <style>
        :root {
            --primary: #4a7a8c;
            --secondary: #6a8caf;
            --accent: #8c7a4a;
            --light: #f0f0f0;
            --dark: #333;
            --danger: #dc3545;
            --success: #28a745;
            --warning: #ffc107;
            --info: #17a2b8;
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Malgun Gothic', '맑은 고딕', sans-serif;
        }
        
        body {
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem;
            text-align: center;
            margin-bottom: 20px;
            border-radius: 5px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .user-info {
            font-size: 0.9rem;
        }
        
        .logout-btn {
            background: var(--secondary);
            color: white;
            border: none;
            padding: 5px 10px;
            border-radius: 3px;
            cursor: pointer;
        }
        
        .login-section {
            background: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        
        .tab-container {
            display: flex;
            margin-bottom: 20px;
            border-bottom: 2px solid var(--primary);
            flex-wrap: wrap;
        }
        
        .tab {
            padding: 10px 20px;
            cursor: pointer;
            background: #e0e0e0;
            margin-right: 5px;
            border-radius: 5px 5px 0 0;
            margin-bottom: 5px;
        }
        
        .tab.active {
            background: var(--primary);
            color: white;
        }
        
        .tab-content {
            display: none;
            background: white;
            padding: 20px;
            border-radius: 0 5px 5px 5px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }
        
        .tab-content.active {
            display: block;
        }
        
        form {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-bottom: 20px;
        }
        
        @media (max-width: 768px) {
            form {
                grid-template-columns: 1fr;
            }
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        
        input, select {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        
        button {
            background-color: var(--primary);
            color: white;
            border: none;
            padding: 10px 15px;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
        
        button:hover {
            background-color: var(--secondary);
        }
        
        button.danger {
            background-color: var(--danger);
        }
        
        button.success {
            background-color: var(--success);
        }
        
        button.warning {
            background-color: var(--warning);
            color: var(--dark);
        }
        
        button.info {
            background-color: var(--info);
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 20px;
        }
        
        th, td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid #ddd;
        }
        
        th {
            background-color: var(--primary);
            color: white;
        }
        
        tr:hover {
            background-color: #f5f5f5;
        }
        
        .metrics {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 20px;
        }
        
        .metric-card {
            background: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            text-align: center;
        }
        
        .metric-value {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary);
        }
        
        footer {
            text-align: center;
            margin-top: 30px;
            padding: 20px;
            background: var(--dark);
            color: white;
            border-radius: 5px;
        }
        
        /* 모바일 대응 */
        @media (max-width: 768px) {
            .container {
                padding: 10px;
            }
            
            .tab {
                padding: 8px 12px;
                font-size: 14px;
            }
            
            th, td {
                padding: 8px 10px;
                font-size: 14px;
            }
            
            header {
                flex-direction: column;
                gap: 10px;
            }
        }
        
        .filter-section {
            background: #f8f9fa;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
        }
        
        .badge {
            display: inline-block;
            padding: 3px 8px;
            border-radius: 12px;
            font-size: 12px;
            font-weight: bold;
        }
        
        .badge-admin {
            background: var(--primary);
            color: white;
        }
        
        .badge-recorder {
            background: var(--secondary);
            color: white;
        }
        
        .import-section {
            background: #e8f4f8;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 20px;
        }
        
        .file-upload {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 10px;
        }
        
        .preview-table {
            max-height: 300px;
            overflow-y: auto;
            margin-top: 15px;
            border: 1px solid #ddd;
        }
        
        .instructions {
            background: #fff3cd;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 15px;
            border-left: 4px solid var(--warning);
        }
        
        .instructions h4 {
            margin-top: 0;
            color: var(--dark);
        }
        
        .instructions ul {
            margin-bottom: 0;
            padding-left: 20px;
        }
        
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 1000;
            justify-content: center;
            align-items: center;
        }
        
        .modal-content {
            background-color: white;
            padding: 20px;
            border-radius: 5px;
            max-width: 500px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
        }
        
        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            border-bottom: 1px solid #ddd;
            padding-bottom: 10px;
        }
        
        .close {
            font-size: 24px;
            cursor: pointer;
        }
        
        .action-buttons {
            display: flex;
            gap: 10px;
            margin-top: 20px;
        }
        
        .error-message {
            color: var(--danger);
            font-size: 14px;
            margin-top: 5px;
        }
        
        .test-account {
            margin-top: 20px;
            padding: 15px;
            background: #f8f9fa;
            border-radius: 5px;
            border-left: 4px solid var(--info);
        }
        
        .loading {
            display: none;
            text-align: center;
            padding: 20px;
        }
        
        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 15px 20px;
            border-radius: 5px;
            color: white;
            z-index: 1000;
            display: none;
        }
        
        .notification.success {
            background-color: var(--success);
        }
        
        .notification.error {
            background-color: var(--danger);
        }
        
        .edit-form {
            background-color: #f8f9fa;
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 15px;
            border-left: 4px solid var(--info);
        }
        
        /* 모바일 최적화 스타일 */
        .mobile-optimized input,
        .mobile-optimized select,
        .mobile-optimized button {
            font-size: 16px; /* iOS zoom 방지 */
            min-height: 44px; /* 터치 최소 크기 */
        }

        .participant-info-card {
            background: #e8f5e8;
            padding: 15px;
            border-radius: 8px;
            border-left: 4px solid #4caf50;
            margin-bottom: 15px;
        }

        .participant-info {
            font-weight: bold;
            color: #2e7d32;
            font-size: 16px;
        }

        .award-preview {
            font-weight: bold;
            padding: 8px 12px;
            border-radius: 4px;
            background: #fff3cd;
            border: 1px solid #ffeaa7;
        }

        .mobile-only {
            display: none;
        }

        @media (max-width: 768px) {
            .mobile-only {
                display: block;
            }
            
            .mobile-action-buttons {
                display: flex;
                flex-direction: column;
                gap: 10px;
            }
            
            .mobile-action-buttons button {
                width: 100%;
                margin: 2px 0;
            }
            
            /* 테이블 스크롤 가능하게 */
            .table-container {
                overflow-x: auto;
                -webkit-overflow-scrolling: touch;
            }
        }

        /* 매우 작은 화면 */
        @media (max-width: 480px) {
            .container {
                padding: 8px !important;
            }
            
            header h1 {
                font-size: 1.3rem !important;
                text-align: center;
            }
            
            .user-info {
                font-size: 0.8rem;
            }
            
            .tab {
                padding: 12px 10px !important;
                font-size: 13px !important;
                margin: 2px;
            }
        }
    </style>
</head>
<body>
    <div class="notification" id="notification"></div>
    
    <div class="container">
        <header id="appHeader" style="display: none;">
            <h1>온라인 줄넘기 대회 관리 시스템</h1>
            <div class="user-info">
                <span id="currentUserInfo"></span>
                <button class="logout-btn" onclick="logout()">로그아웃</button>
            </div>
        </header>
        
        <section class="login-section" id="loginSection">
            <h2>로그인</h2>
            <form id="loginForm">
                <div class="form-group">
                    <label for="username">사용자명</label>
                    <input type="text" id="username" required>
                </div>
                <div class="form-group">
                    <label for="password">비밀번호</label>
                    <input type="password" id="password" required>
                </div>
                <button type="submit">로그인</button>
                <div id="loginError" class="error-message" style="display: none;"></div>
            </form>
            
            <div class="test-account">
                <h4>테스트 계정 정보</h4>
                <p><strong>관리자 :</strong> jong yun</p>
                <p><strong>기록담당자 계정:</strong> 폰 / 번호 </p>
                <p>데모를 위해 위 계정으로 로그인하세요.</p>
            </div>
        </section>
        
        <div class="loading" id="loading">
            <p>데이터를 불러오는 중입니다...</p>
        </div>
        
        <main id="mainApp" style="display: none;">
            <div class="tab-container">
                <div class="tab active" data-tab="dashboard">대시보드</div>
                <div class="tab" data-tab="participants">참가자 관리</div>
                <div class="tab" data-tab="scores">경기 기록</div>
                <div class="tab" data-tab="rankings">순위 현황</div>
                <div class="tab" data-tab="criteria">시상 기준</div>
                <div class="tab" data-tab="users" id="usersTab">사용자 관리</div>
            </div>
            
            <div class="tab-content active" id="dashboard">
                <h2>대시보드</h2>
                <div class="metrics">
                    <div class="metric-card">
                        <div class="metric-label">총 참가자</div>
                        <div class="metric-value" id="totalParticipants">0</div>
                    </div>
                    <div class="metric-card">
                        <div class="metric-label">총 경기수</div>
                        <div class="metric-value" id="totalMatches">0</div>
                    </div>
                    <div class="metric-card">
                        <div class="metric-label">총 수상자</div>
                        <div class="metric-value" id="totalWinners">0</div>
                    </div>
                    <div class="metric-card">
                        <div class="metric-label">활동 심판</div>
                        <div class="metric-value" id="activeJudges">0</div>
                    </div>
                </div>
                
                <h3>최근 시상 기록</h3>
                <table>
                    <thead>
                        <tr>
                            <th>번호</th>
                            <th>이름</th>
                            <th>종목</th>
                            <th>참가부</th>
                            <th>수상</th>
                            <th>소속</th>
                        </tr>
                    </thead>
                    <tbody id="recentAwards">
                        <!-- 최근 시상 기록이 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
            </div>
            
            <div class="tab-content" id="participants">
                <h2>참가자 관리</h2>
                
                <div class="import-section">
                    <h3>엑셀 일괄 등록</h3>
                    <div class="instructions">
                        <h4>엑셀 파일 형식 안내</h4>
                        <ul>
                            <li>파일 형식: .xlsx 또는 .xls</li>
                            <li>열 순서: 번호, 이름, 소속, 참가부</li>
                            <li>첫 행은 헤더로 사용 (예: A1:번호, B1:이름, C1:소속, D1:참가부)</li>
                            <li>참가부: 유치부, 초등1부, 초등2부, 초등3부, 초등4부, 초등5부, 초등6부, 중등부, 고등부, 일반부, 선수</li>
                        </ul>
                    </div>
                    
                    <div class="file-upload">
                        <input type="file" id="excelFile" accept=".xlsx, .xls">
                        <button onclick="previewExcel()" class="info">미리보기</button>
                    </div>
                    
                    <div id="excelPreview" class="preview-table" style="display: none;">
                        <table>
                            <thead id="previewHeader">
                                <tr>
                                    <th>번호</th>
                                    <th>이름</th>
                                    <th>소속</th>
                                    <th>참가부</th>
                                    <th>상태</th>
                                </tr>
                            </thead>
                            <tbody id="previewBody">
                                <!-- 미리보기 데이터가 여기에 표시됩니다 -->
                            </tbody>
                        </table>
                    </div>
                    
                    <div class="action-buttons">
                        <button onclick="importExcel()" class="success" id="importBtn" style="display: none;">일괄 등록</button>
                        <button onclick="downloadTemplate()" class="warning">엑셀 템플릿 다운로드</button>
                    </div>
                </div>
                
                <h3>참가자 수동 등록</h3>
                <form id="participantForm">
                    <div class="form-group">
                        <label for="participantId">참가자 번호</label>
                        <input type="text" id="participantId" required>
                    </div>
                    <div class="form-group">
                        <label for="participantName">이름</label>
                        <input type="text" id="participantName" required>
                    </div>
                    <div class="form-group">
                        <label for="participantTeam">소속</label>
                        <input type="text" id="participantTeam" required>
                    </div>
                    <div class="form-group">
                        <label for="participantGrade">참가부</label>
                        <select id="participantGrade" required>
                            <option value="유치부">유치부</option>
                            <option value="초등1부">초등1부</option>
                            <option value="초등2부">초등2부</option>
                            <option value="초등3부">초등3부</option>
                            <option value="초등4부">초등4부</option>
                            <option value="초등5부">초등5부</option>
                            <option value="초등6부">초등6부</option>
                            <option value="중등부">중등부</option>
                            <option value="고등부">고등부</option>
                            <option value="일반부">일반부</option>
                            <option value="선수">선수</option>
                        </select>
                    </div>
                    <button type="submit">참가자 추가</button>
                </form>
                
                <h3>참가자 목록</h3>
                <div class="filter-section">
                    <div class="form-group">
                        <label for="participantFilterTeam">소속 필터</label>
                        <input type="text" id="participantFilterTeam" placeholder="소속명으로 필터">
                    </div>
                    <div class="form-group">
                        <label for="participantFilterGrade">참가부 필터</label>
                        <select id="participantFilterGrade">
                            <option value="">전체 부문</option>
                            <option value="유치부">유치부</option>
                            <option value="초등1부">초등1부</option>
                            <option value="초등2부">초등2부</option>
                            <option value="초등3부">초등3부</option>
                            <option value="초등4부">초등4부</option>
                            <option value="초등5부">초등5부</option>
                            <option value="초등6부">초등6부</option>
                            <option value="중등부">중등부</option>
                            <option value="고등부">고등부</option>
                            <option value="일반부">일반부</option>
                            <option value="선수">선수</option>
                        </select>
                    </div>
                </div>
                <table>
                    <thead>
                        <tr>
                            <th>번호</th>
                            <th>이름</th>
                            <th>소속</th>
                            <th>참가부</th>
                            <th>작업</th>
                        </tr>
                    </thead>
                    <tbody id="participantsList">
                        <!-- 참가자 목록이 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
            </div>
            
            <div class="tab-content" id="scores">
                <h2>📱 경기 기록 입력</h2>
                
                <!-- 빠른 입력 가이드 -->
                <div class="instructions mobile-only" style="display: none;">
                    <h4>모바일 사용 가이드</h4>
                    <ul>
                        <li>참가자 번호 입력 후 자동 검색</li>
                        <li>점수 입력 후 엔터키로 빠른 저장</li>
                        <li>ESC 키로 입력 초기화</li>
                    </ul>
                </div>
                
                <form id="scoreForm" class="mobile-optimized">
                    <div class="form-group">
                        <label for="scoreParticipantId">🔍 참가자 번호</label>
                        <input type="text" id="scoreParticipantId" placeholder="번호 입력 후 자동 검색" required>
                        <small class="form-text">3자 이상 입력 시 자동 검색</small>
                    </div>
                    
                    <div class="participant-info-card" id="participantInfoCard" style="display: none;">
                        <div class="form-group">
                            <label>선수 정보</label>
                            <div id="participantInfoLabel" class="participant-info"></div>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="scoreEvent">🎯 경기 종목</label>
                        <select id="scoreEvent" required>
                            <option value="">종목 선택</option>
                            <option value="양발모아뛰기">양발모아뛰기</option>
                            <option value="30초 번갈아뛰기">30초 번갈아뛰기</option>
                            <option value="30초 이중뛰기">30초 이중뛰기</option>
                            <option value="2인 맞서뛰기1분">2인 맞서뛰기1분</option>
                            <option value="2인 스피드릴레이1분">2인 스피드릴레이1분</option>
                            <option value="2인번갈아뛰기">2인번갈아뛰기</option>
                            <option value="3중 뛰기">3중 뛰기</option>
                            <option value="8자마라톤">8자마라톤</option>
                            <option value="긴줄다함께뛰기">긴줄다함께뛰기</option>
                            <option value="가족3인 릴레이">가족3인 릴레이</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="scoreValue">⭐ 점수</label>
                        <input type="number" id="scoreValue" step="0.1" placeholder="점수 입력" required>
                    </div>
                    
                    <div class="form-group">
                        <label>🏆 예상 수상</label>
                        <div id="awardLabel" class="award-preview">-</div>
                    </div>
                    
                    <div class="mobile-action-buttons">
                        <button type="submit" class="success">💾 기록 저장 (Enter)</button>
                        <button type="button" onclick="clearScoreForm()" class="warning">🔄 초기화 (ESC)</button>
                    </div>
                </form>
                
                <h3>경기 기록</h3>
                <div class="filter-section">
                    <div class="form-group">
                        <label for="scoreFilterEvent">종목 필터</label>
                        <select id="scoreFilterEvent">
                            <option value="">전체 종목</option>
                            <option value="양발모아뛰기">양발모아뛰기</option>
                            <option value="30초 번갈아뛰기">30초 번갈아뛰기</option>
                            <option value="30초 이중뛰기">30초 이중뛰기</option>
                            <option value="2인 맞서뛰기1분">2인 맞서뛰기1분</option>
                            <option value="2인 스피드릴레이1분">2인 스피드릴레이1분</option>
                            <option value="2인번갈아뛰기">2인번갈아뛰기</option>
                            <option value="3중 뛰기">3중 뛰기</option>
                            <option value="8자마라톤">8자마라톤</option>
                            <option value="긴줄다함께뛰기">긴줄다함께뛰기</option>
                            <option value="가족3인 릴레이">가족3인 릴레이</option>
                        </select>
                    </div>
                </div>
                <table>
                    <thead>
                        <tr>
                            <th>참가자 번호</th>
                            <th>이름</th>
                            <th>경기 종목</th>
                            <th>참가부</th>
                            <th>점수</th>
                            <th>수상</th>
                            <th>작업</th>
                        </tr>
                    </thead>
                    <tbody id="scoresList">
                        <!-- 경기 기록이 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
            </div>
            
            <div class="tab-content" id="rankings">
                <h2>순위 현황</h2>
                <div class="filter-section">
                    <div class="form-group">
                        <label for="rankingFilter">부문 필터</label>
                        <select id="rankingFilter">
                            <option value="">전체</option>
                            <option value="유치부">유치부</option>
                            <option value="초등1부">초등1부</option>
                            <option value="초등2부">초등2부</option>
                            <option value="초등3부">초등3부</option>
                            <option value="초등4부">초등4부</option>
                            <option value="초등5부">초등5부</option>
                            <option value="초등6부">초등6부</option>
                            <option value="중등부">중등부</option>
                            <option value="고등부">고등부</option>
                            <option value="일반부">일반부</option>
                            <option value="선수">선수</option>
                        </select>
                    </div>
                </div>
                
                <h3>개인 순위</h3>
                <table>
                    <thead>
                        <tr>
                            <th>순위</th>
                            <th>이름</th>
                            <th>소속</th>
                            <th>참가부</th>
                            <th>대상</th>
                            <th>금</th>
                            <th>은</th>
                            <th>동</th>
                            <th>총점</th>
                        </tr>
                    </thead>
                    <tbody id="individualRankings">
                        <!-- 개인 순위가 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
                
                <h3>단체 순위</h3>
                <table>
                    <thead>
                        <tr>
                            <th>순위</th>
                            <th>소속</th>
                            <th>대상</th>
                            <th>금</th>
                            <th>은</th>
                            <th>동</th>
                            <th>총점</th>
                        </tr>
                    </thead>
                    <tbody id="teamRankings">
                        <!-- 단체 순위가 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
            </div>
            
            <div class="tab-content" id="criteria">
                <h2>시상 기준 관리</h2>
                <form id="criteriaForm">
                    <div class="form-group">
                        <label for="criteriaEvent">경기 종목</label>
                        <select id="criteriaEvent" required>
                            <option value="양발모아뛰기">양발모아뛰기</option>
                            <option value="30초 번갈아뛰기">30초 번갈아뛰기</option>
                            <option value="30초 이중뛰기">30초 이중뛰기</option>
                            <option value="2인 맞서뛰기1분">2인 맞서뛰기1분</option>
                            <option value="2인 스피드릴레이1분">2인 스피드릴레이1분</option>
                            <option value="2인번갈아뛰기">2인번갈아뛰기</option>
                            <option value="3중 뛰기">3중 뛰기</option>
                            <option value="8자마라톤">8자마라톤</option>
                            <option value="긴줄다함께뛰기">긴줄다함께뛰기</option>
                            <option value="가족3인 릴레이">가족3인 릴레이</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="criteriaGrade">참가부</label>
                        <select id="criteriaGrade" required>
                            <option value="전체">전체 부문</option>
                            <option value="유치부">유치부</option>
                            <option value="초등1부">초등1부</option>
                            <option value="초등2부">초등2부</option>
                            <option value="초등3부">초등3부</option>
                            <option value="초등4부">초등4부</option>
                            <option value="초등5부">초등5부</option>
                            <option value="초등6부">초등6부</option>
                            <option value="중등부">중등부</option>
                            <option value="고등부">고등부</option>
                            <option value="일반부">일반부</option>
                            <option value="선수">선수</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="criteriaGold">금상 기준</label>
                        <input type="number" id="criteriaGold" step="0.1" required>
                    </div>
                    <div class="form-group">
                        <label for="criteriaSilver">은상 기준</label>
                        <input type="number" id="criteriaSilver" step="0.1" required>
                    </div>
                    <div class="form-group">
                        <label for="criteriaBronze">동상 기준</label>
                        <input type="number" id="criteriaBronze" step="0.1" required>
                    </div>
                    <button type="submit">기준 저장</button>
                </form>
                
                <h3>시상 기준 목록</h3>
                <div class="filter-section">
                    <div class="form-group">
                        <label for="criteriaFilterEvent">종목 필터</label>
                        <select id="criteriaFilterEvent">
                            <option value="">전체 종목</option>
                            <option value="양발모아뛰기">양발모아뛰기</option>
                            <option value="30초 번갈아뛰기">30초 번갈아뛰기</option>
                            <option value="30초 이중뛰기">30초 이중뛰기</option>
                            <option value="2인 맞서뛰기1분">2인 맞서뛰기1분</option>
                            <option value="2인 스피드릴레이1분">2인 스피드릴레이1분</option>
                            <option value="2인번갈아뛰기">2인번갈아뛰기</option>
                            <option value="3중 뛰기">3중 뛰기</option>
                            <option value="8자마라톤">8자마라톤</option>
                            <option value="긴줄다함께뛰기">긴줄다함께뛰기</option>
                            <option value="가족3인 릴레이">가족3인 릴레이</option>
                        </select>
                    </div>
                </div>
                <table>
                    <thead>
                        <tr>
                            <th>경기 종목</th>
                            <th>참가부</th>
                            <th>금상 기준</th>
                            <th>은상 기준</th>
                            <th>동상 기준</th>
                            <th>작업</th>
                        </tr>
                    </thead>
                    <tbody id="criteriaList">
                        <!-- 시상 기준이 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
            </div>
            
            <div class="tab-content" id="users">
                <h2>사용자 관리</h2>
                
                <!-- 사용자 수정 폼 (기본적으로 숨김) -->
                <div id="userEditForm" class="edit-form" style="display: none;">
                    <h3>사용자 정보 수정</h3>
                    <form id="editUserForm">
                        <input type="hidden" id="editUsername">
                        <div class="form-group">
                            <label for="editPassword">새 비밀번호</label>
                            <input type="password" id="editPassword">
                        </div>
                        <div class="form-group">
                            <label for="editUserRole">역할</label>
                            <select id="editUserRole" required>
                                <option value="admin">관리자</option>
                                <option value="recorder">기록 담당자(심판)</option>
                            </select>
                        </div>
                        <button type="submit" class="success">수정 완료</button>
                        <button type="button" onclick="cancelEditUser()" class="warning">취소</button>
                    </form>
                </div>
                
                <form id="userForm">
                    <div class="form-group">
                        <label for="newUsername">사용자명</label>
                        <input type="text" id="newUsername" required>
                    </div>
                    <div class="form-group">
                        <label for="newPassword">비밀번호</label>
                        <input type="password" id="newPassword" required>
                    </div>
                    <div class="form-group">
                        <label for="newUserRole">역할</label>
                        <select id="newUserRole" required>
                            <option value="admin">관리자</option>
                            <option value="recorder">기록 담당자(심판)</option>
                        </select>
                    </div>
                    <button type="submit">사용자 추가</button>
                </form>
                
                <h3>사용자 목록</h3>
                <table>
                    <thead>
                        <tr>
                            <th>사용자명</th>
                            <th>역할</th>
                            <th>작업</th>
                        </tr>
                    </thead>
                    <tbody id="usersList">
                        <!-- 사용자 목록이 여기에 동적으로 추가됩니다 -->
                    </tbody>
                </table>
            </div>
        </main>
        
        <!-- 모달 창 -->
        <div id="importModal" class="modal">
            <div class="modal-content">
                <div class="modal-header">
                    <h3>엑셀 일괄 등록 결과</h3>
                    <span class="close" onclick="closeModal()">&times;</span>
                </div>
                <div id="modalBody">
                    <!-- 모달 내용이 여기에 표시됩니다 -->
                </div>
                <div class="action-buttons">
                    <button onclick="closeModal()" class="success">확인</button>
                </div>
            </div>
        </div>
        
        <footer>
            <p>© 2024 대한 줄넘기협회 대회 관리 시스템. All rights reserved.</p>
        </footer>
    </div>

    <script>
        // 데이터 저장
        let participants = JSON.parse(localStorage.getItem('participants')) || [];
        let scores = JSON.parse(localStorage.getItem('scores')) || [];
        let results = JSON.parse(localStorage.getItem('results')) || [];
        let awardCriteria = JSON.parse(localStorage.getItem('awardCriteria')) || {};
        let users = JSON.parse(localStorage.getItem('users')) || [];
        let currentUser = null;
        let currentParticipant = null;
        let excelData = []; // 엑셀 미리보기 데이터 저장
        let editingUser = null; // 현재 수정 중인 사용자
        
        // 초기 데이터 설정
        function initializeData() {
            // 사용자 데이터가 없으면 기본 계정들 생성
            if (users.length === 0) {
                users = [
                    { username: 'admin', password: 'admin123', role: 'admin' },
                    { username: 'recorder', password: 'recorder123', role: 'recorder' }
                ];
                localStorage.setItem('users', JSON.stringify(users));
            } else {
                // 기존 사용자 데이터 로드
                users = JSON.parse(localStorage.getItem('users'));
            }
            
            // 시상 기준 데이터가 없으면 기본값 설정
            if (Object.keys(awardCriteria).length === 0) {
                awardCriteria = {
                    '양발모아뛰기': {
                        '전체': { gold: 100, silver: 80, bronze: 60 }
                    }
                };
                localStorage.setItem('awardCriteria', JSON.stringify(awardCriteria));
            } else {
                awardCriteria = JSON.parse(localStorage.getItem('awardCriteria'));
            }
        }
        
        // 자동 검색 설정
        function setupAutoSearch() {
            const participantIdInput = document.getElementById('scoreParticipantId');
            
            // 엔터 키로 검색
            participantIdInput.addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    findParticipant();
                }
            });
            
            // 입력 후 일정 시간 지나면 자동 검색 (디바운스)
            let timeoutId;
            participantIdInput.addEventListener('input', function() {
                clearTimeout(timeoutId);
                timeoutId = setTimeout(() => {
                    if (this.value.length >= 3) { // 3자 이상 입력시 자동 검색
                        findParticipant();
                    }
                }, 500);
            });
        }
        
        // 역할 기반 UI 제한
        function setupRoleBasedUI() {
            if (currentUser.role !== 'admin') {
                // 기록 담당자는 경기 기록 탭만 보이도록
                document.querySelectorAll('.tab').forEach(tab => {
                    if (tab.dataset.tab !== 'scores') {
                        tab.style.display = 'none';
                    }
                });
                
                // 경기 기록 탭으로 자동 이동
                switchTab('scores');
                
                // 모바일 최적화 스타일 적용
                applyMobileOptimizations();
            }
        }
        
        // 모바일 최적화 스타일
        function applyMobileOptimizations() {
            const style = document.createElement('style');
            style.textContent = `
                @media (max-width: 768px) {
                    /* 모바일에서 더 큰 터치 영역 */
                    .mobile-optimized input,
                    .mobile-optimized select,
                    .mobile-optimized button {
                        font-size: 16px !important; /* iOS zoom 방지 */
                        min-height: 44px !important;
                        padding: 12px 8px !important;
                    }
                    
                    /* 경기 기록 입력 폼 모바일 최적화 */
                    #scoreForm {
                        grid-template-columns: 1fr !important;
                        gap: 10px !important;
                    }
                    
                    .form-group {
                        margin-bottom: 15px !important;
                    }
                    
                    /* 테이블 모바일 친화적으로 */
                    table {
                        font-size: 14px;
                    }
                    
                    th, td {
                        padding: 8px 4px !important;
                    }
                    
                    /* 액션 버튼 모바일 최적화 */
                    .mobile-action-buttons {
                        display: flex;
                        flex-direction: column;
                        gap: 8px;
                    }
                    
                    .mobile-action-buttons button {
                        width: 100%;
                        margin: 2px 0;
                    }
                }
                
                /* 매우 작은 화면 대응 */
                @media (max-width: 480px) {
                    .container {
                        padding: 5px !important;
                    }
                    
                    header h1 {
                        font-size: 1.2rem !important;
                    }
                    
                    .tab {
                        padding: 10px 8px !important;
                        font-size: 12px !important;
                    }
                }
            `;
            document.head.appendChild(style);
            
            // 모바일 최적화 클래스 추가
            document.getElementById('scoreForm').classList.add('mobile-optimized');
            document.querySelectorAll('#scores button').forEach(btn => {
                btn.parentElement.classList.add('mobile-action-buttons');
            });
            
            // 모바일 감지 시 모바일 가이드 표시
            if (/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
                document.querySelector('.mobile-only').style.display = 'block';
            }
        }
        
        // 모바일에서의 빠른 입력을 위한 단축키
        function setupMobileShortcuts() {
            document.addEventListener('keydown', function(e) {
                // 기록 담당자 모드에서만 적용
                if (currentUser.role !== 'admin') {
                    // 엔터 키로 빠른 제출
                    if (e.key === 'Enter' && e.target.tagName !== 'TEXTAREA') {
                        const activeElement = document.activeElement;
                        if (activeElement.id === 'scoreValue') {
                            document.getElementById('scoreForm').dispatchEvent(new Event('submit'));
                        }
                    }
                    
                    // ESC 키로 폼 초기화
                    if (e.key === 'Escape') {
                        clearScoreForm();
                        document.getElementById('scoreParticipantId').focus();
                    }
                }
            });
        }
        
        // 참가자 찾기 함수 개선
        function findParticipant() {
            const participantId = document.getElementById('scoreParticipantId').value.trim().toUpperCase();
            
            if (!participantId) {
                showNotification('참가자 번호를 입력해주세요.', 'error');
                return;
            }
            
            try {
                const participant = participants.find(p => p.id.toUpperCase() === participantId);
                if (participant) {
                    currentParticipant = participant;
                    document.getElementById('participantInfoLabel').textContent = 
                        `${participant.name} (${participant.team}, ${participant.grade})`;
                    
                    // 참가자 정보 카드 표시
                    document.getElementById('participantInfoCard').style.display = 'block';
                    
                    // 해당 참가자의 경기 기록 강조 표시
                    highlightParticipantScores(participantId);
                    
                    // 점수 입력 필드로 자동 포커스
                    document.getElementById('scoreValue').focus();
                    
                    showNotification(`참가자 찾기 완료: ${participant.name}`, 'success');
                } else {
                    showNotification('해당 번호의 참가자를 찾을 수 없습니다.', 'error');
                    resetParticipantInfo();
                }
            } catch (error) {
                showNotification('참가자 찾기 중 오류가 발생했습니다.', 'error');
                console.error('참가자 찾기 오류:', error);
            }
        }
        
        // 참가자 정보 초기화
        function resetParticipantInfo() {
            currentParticipant = null;
            document.getElementById('participantInfoLabel').textContent = '';
            document.getElementById('participantInfoCard').style.display = 'none';
            document.getElementById('scoreValue').value = '';
            document.getElementById('awardLabel').textContent = '-';
        }
        
        // 참가자 기록 강조 표시
        function highlightParticipantScores(participantId) {
            const scoresList = document.getElementById('scoresList');
            const rows = scoresList.getElementsByTagName('tr');
            
            // 모든 행의 강조 제거
            for (let row of rows) {
                row.style.backgroundColor = '';
            }
            
            // 해당 참가자의 행 강조
            for (let row of rows) {
                const cells = row.getElementsByTagName('td');
                if (cells.length > 0 && cells[0].textContent.toUpperCase() === participantId) {
                    row.style.backgroundColor = '#e8f5e8';
                }
            }
        }
        
        // 로그인 처리
        document.getElementById('loginForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const username = document.getElementById('username').value;
            const password = document.getElementById('password').value;
            
            const user = users.find(u => u.username === username && u.password === password);
            
            if (user) {
                currentUser = user;
                localStorage.setItem('currentUser', JSON.stringify(user));
                showNotification('로그인 성공!', 'success');
                loadApp();
            } else {
                document.getElementById('loginError').textContent = '사용자명 또는 비밀번호가 올바르지 않습니다.';
                document.getElementById('loginError').style.display = 'block';
                showNotification('로그인 실패: 사용자명 또는 비밀번호가 올바르지 않습니다.', 'error');
            }
        });
        
        // 로그아웃
        function logout() {
            currentUser = null;
            localStorage.removeItem('currentUser');
            document.getElementById('loginSection').style.display = 'block';
            document.getElementById('appHeader').style.display = 'none';
            document.getElementById('mainApp').style.display = 'none';
            document.getElementById('username').value = '';
            document.getElementById('password').value = '';
            document.getElementById('loginError').style.display = 'none';
        }
        
        // 앱 로드
        function loadApp() {
            document.getElementById('loginSection').style.display = 'none';
            document.getElementById('appHeader').style.display = 'flex';
            document.getElementById('mainApp').style.display = 'block';
            
            // 현재 사용자 정보 표시
            document.getElementById('currentUserInfo').innerHTML = `
                ${currentUser.username} 
                <span class="badge ${currentUser.role === 'admin' ? 'badge-admin' : 'badge-recorder'}">
                    ${currentUser.role === 'admin' ? '관리자' : '기록담당자'}
                </span>
            `;
            
            // 역할 기반 UI 설정
            setupRoleBasedUI();
            
            // 자동 검색 설정
            setupAutoSearch();
            
            // 모바일 단축키 설정
            setupMobileShortcuts();
            
            // 데이터 로드
            loadParticipants();
            loadScores();
            loadRankings();
            loadCriteria();
            loadUsers();
            updateDashboard();
            
            // 탭 전환 이벤트 설정
            setupTabEvents();
            
            showNotification(`${currentUser.username}님, 환영합니다!`, 'success');
        }
        
        // 탭 전환 함수
        function switchTab(tabName) {
            // 모든 탭 비활성화
            document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
            document.querySelectorAll('.tab-content').forEach(c => c.classList.remove('active'));
            
            // 선택한 탭 활성화
            const selectedTab = document.querySelector(`[data-tab="${tabName}"]`);
            if (selectedTab) {
                selectedTab.classList.add('active');
                document.getElementById(tabName).classList.add('active');
            }
        }
        
        function setupTabEvents() {
            document.querySelectorAll('.tab').forEach(tab => {
                tab.addEventListener('click', function() {
                    if (currentUser.role === 'admin' || this.dataset.tab === 'scores') {
                        switchTab(this.dataset.tab);
                    } else {
                        showNotification('접근 권한이 없습니다.', 'error');
                    }
                });
            });
        }
        
        // 대시보드 업데이트
        function updateDashboard() {
            // 총 참가자 수
            document.getElementById('totalParticipants').textContent = participants.length;
            
            // 총 경기 수
            document.getElementById('totalMatches').textContent = scores.length;
            
            // 총 수상자 수
            const totalWinners = results.filter(r => r.award !== '없음').length;
            document.getElementById('totalWinners').textContent = totalWinners;
            
            // 활동 심판 수
            const activeJudges = [...new Set(scores.map(s => s.judge))].length;
            document.getElementById('activeJudges').textContent = activeJudges;
            
            // 최근 시상 기록
            const recentAwards = results
                .filter(r => r.award !== '없음')
                .sort((a, b) => new Date(b.date) - new Date(a.date))
                .slice(0, 10);
            
            const recentAwardsHtml = recentAwards.map((result, index) => {
                const participant = participants.find(p => p.id === result.participantId);
                return `
                    <tr>
                        <td>${index + 1}</td>
                        <td>${participant ? participant.name : '알 수 없음'}</td>
                        <td>${result.event}</td>
                        <td>${participant ? participant.grade : '알 수 없음'}</td>
                        <td>${result.award}</td>
                        <td>${participant ? participant.team : '알 수 없음'}</td>
                    </tr>
                `;
            }).join('');
            
            document.getElementById('recentAwards').innerHTML = recentAwardsHtml || '<tr><td colspan="6">최근 시상 기록이 없습니다.</td></tr>';
        }
        
        // 참가자 로드
        function loadParticipants() {
            const participantsList = document.getElementById('participantsList');
            const teamFilter = document.getElementById('participantFilterTeam').value.toLowerCase();
            const gradeFilter = document.getElementById('participantFilterGrade').value;
            
            let filteredParticipants = participants;
            
            if (teamFilter) {
                filteredParticipants = filteredParticipants.filter(p => p.team.toLowerCase().includes(teamFilter));
            }
            
            if (gradeFilter) {
                filteredParticipants = filteredParticipants.filter(p => p.grade === gradeFilter);
            }
            
            const participantsHtml = filteredParticipants.map(participant => `
                <tr>
                    <td>${participant.id}</td>
                    <td>${participant.name}</td>
                    <td>${participant.team}</td>
                    <td>${participant.grade}</td>
                    <td>
                        <button onclick="deleteParticipant('${participant.id}')" class="danger">삭제</button>
                    </td>
                </tr>
            `).join('');
            
            participantsList.innerHTML = participantsHtml || '<tr><td colspan="5">등록된 참가자가 없습니다.</td></tr>';
        }
        
        // 참가자 추가
        document.getElementById('participantForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const id = document.getElementById('participantId').value;
            const name = document.getElementById('participantName').value;
            const team = document.getElementById('participantTeam').value;
            const grade = document.getElementById('participantGrade').value;
            
            // 중복 ID 확인
            if (participants.some(p => p.id === id)) {
                showNotification('이미 존재하는 참가자 번호입니다.', 'error');
                return;
            }
            
            participants.push({ id, name, team, grade });
            localStorage.setItem('participants', JSON.stringify(participants));
            
            showNotification('참가자가 성공적으로 추가되었습니다.', 'success');
            loadParticipants();
            updateDashboard();
            
            // 폼 초기화
            document.getElementById('participantForm').reset();
        });
        
        // 참가자 삭제
        function deleteParticipant(id) {
            if (confirm('정말로 이 참가자를 삭제하시겠습니까? 관련된 모든 기록도 함께 삭제됩니다.')) {
                // 참가자 삭제
                participants = participants.filter(p => p.id !== id);
                localStorage.setItem('participants', JSON.stringify(participants));
                
                // 관련 기록 삭제
                scores = scores.filter(s => s.participantId !== id);
                localStorage.setItem('scores', JSON.stringify(scores));
                
                // 관련 결과 삭제
                results = results.filter(r => r.participantId !== id);
                localStorage.setItem('results', JSON.stringify(results));
                
                showNotification('참가자가 삭제되었습니다.', 'success');
                loadParticipants();
                loadScores();
                updateDashboard();
            }
        }
        
        // 경기 기록 로드
        function loadScores() {
            const scoresList = document.getElementById('scoresList');
            const eventFilter = document.getElementById('scoreFilterEvent').value;
            
            let filteredScores = scores;
            
            if (eventFilter) {
                filteredScores = filteredScores.filter(s => s.event === eventFilter);
            }
            
            const scoresHtml = filteredScores.map(score => {
                const participant = participants.find(p => p.id === score.participantId);
                const result = results.find(r => r.participantId === score.participantId && r.event === score.event);
                
                return `
                    <tr>
                        <td>${score.participantId}</td>
                        <td>${participant ? participant.name : '알 수 없음'}</td>
                        <td>${score.event}</td>
                        <td>${participant ? participant.grade : '알 수 없음'}</td>
                        <td>${score.value}</td>
                        <td>${result ? result.award : '없음'}</td>
                        <td>
                            <button onclick="deleteScore('${score.participantId}', '${score.event}')" class="danger">삭제</button>
                        </td>
                    </tr>
                `;
            }).join('');
            
            scoresList.innerHTML = scoresHtml || '<tr><td colspan="7">등록된 경기 기록이 없습니다.</td></tr>';
        }
        
        // 경기 기록 추가
        document.getElementById('scoreForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const participantId = document.getElementById('scoreParticipantId').value;
            const event = document.getElementById('scoreEvent').value;
            const value = parseFloat(document.getElementById('scoreValue').value);
            
            // 참가자 존재 여부 확인
            if (!participants.some(p => p.id === participantId)) {
                showNotification('존재하지 않는 참가자 번호입니다.', 'error');
                return;
            }
            
            // 중복 기록 확인 (동일 참가자의 동일 종목)
            if (scores.some(s => s.participantId === participantId && s.event === event)) {
                showNotification('이미 해당 참가자의 이 종목 기록이 존재합니다.', 'error');
                return;
            }
            
            scores.push({
                participantId,
                event,
                value,
                judge: currentUser.username,
                date: new Date().toISOString()
            });
            
            localStorage.setItem('scores', JSON.stringify(scores));
            
            // 결과 업데이트
            updateResults(participantId, event, value);
            
            showNotification('경기 기록이 성공적으로 추가되었습니다.', 'success');
            loadScores();
            updateDashboard();
            
            // 폼 초기화
            clearScoreForm();
        });
        
        // 경기 기록 삭제
        function deleteScore(participantId, event) {
            if (confirm('정말로 이 경기 기록을 삭제하시겠습니까?')) {
                scores = scores.filter(s => !(s.participantId === participantId && s.event === event));
                localStorage.setItem('scores', JSON.stringify(scores));
                
                // 결과도 함께 삭제
                results = results.filter(r => !(r.participantId === participantId && r.event === event));
                localStorage.setItem('results', JSON.stringify(results));
                
                showNotification('경기 기록이 삭제되었습니다.', 'success');
                loadScores();
                updateDashboard();
            }
        }
        
        // 점수 입력 폼 초기화
        function clearScoreForm() {
            document.getElementById('scoreValue').value = '';
            document.getElementById('awardLabel').textContent = '-';
            document.getElementById('scoreParticipantId').focus();
        }
        
        // 결과 업데이트
        function updateResults(participantId, event, value) {
            const participant = participants.find(p => p.id === participantId);
            if (!participant) return;
            
            // 해당 종목과 부문의 시상 기준 찾기
            let criteria = awardCriteria[event]?.[participant.grade] || awardCriteria[event]?.['전체'];
            
            if (!criteria) {
                // 기본 시상 기준
                criteria = { gold: 100, silver: 80, bronze: 60 };
            }
            
            // 수상 등급 결정
            let award = '없음';
            if (value >= criteria.gold) {
                award = '대상';
            } else if (value >= criteria.silver) {
                award = '금상';
            } else if (value >= criteria.bronze) {
                award = '은상';
            } else if (value > 0) {
                award = '동상';
            }
            
            // 기존 결과 삭제
            results = results.filter(r => !(r.participantId === participantId && r.event === event));
            
            // 새 결과 추가
            results.push({
                participantId,
                event,
                award,
                date: new Date().toISOString()
            });
            
            localStorage.setItem('results', JSON.stringify(results));
        }
        
        // 순위 로드
        function loadRankings() {
            loadIndividualRankings();
            loadTeamRankings();
        }
        
        // 개인 순위 로드
        function loadIndividualRankings() {
            const individualRankings = document.getElementById('individualRankings');
            const gradeFilter = document.getElementById('rankingFilter').value;
            
            // 개인별 수상 내역 집계
            const individualStats = {};
            
            participants.forEach(participant => {
                if (gradeFilter && participant.grade !== gradeFilter) return;
                
                const participantResults = results.filter(r => r.participantId === participant.id);
                
                individualStats[participant.id] = {
                    name: participant.name,
                    team: participant.team,
                    grade: participant.grade,
                    daesang: participantResults.filter(r => r.award === '대상').length,
                    gold: participantResults.filter(r => r.award === '금상').length,
                    silver: participantResults.filter(r => r.award === '은상').length,
                    bronze: participantResults.filter(r => r.award === '동상').length,
                    total: 0
                };
                
                // 점수 계산 (대상:4, 금:3, 은:2, 동:1)
                individualStats[participant.id].total = 
                    individualStats[participant.id].daesang * 4 +
                    individualStats[participant.id].gold * 3 +
                    individualStats[participant.id].silver * 2 +
                    individualStats[participant.id].bronze;
            });
            
            // 총점으로 정렬
            const sortedStats = Object.values(individualStats)
                .filter(stat => stat.total > 0)
                .sort((a, b) => b.total - a.total);
            
            const rankingsHtml = sortedStats.map((stat, index) => `
                <tr>
                    <td>${index + 1}</td>
                    <td>${stat.name}</td>
                    <td>${stat.team}</td>
                    <td>${stat.grade}</td>
                    <td>${stat.daesang}</td>
                    <td>${stat.gold}</td>
                    <td>${stat.silver}</td>
                    <td>${stat.bronze}</td>
                    <td>${stat.total}</td>
                </tr>
            `).join('');
            
            individualRankings.innerHTML = rankingsHtml || '<tr><td colspan="9">순위 데이터가 없습니다.</td></tr>';
        }
        
        // 단체 순위 로드
        function loadTeamRankings() {
            const teamRankings = document.getElementById('teamRankings');
            const gradeFilter = document.getElementById('rankingFilter').value;
            
            // 단체별 수상 내역 집계
            const teamStats = {};
            
            participants.forEach(participant => {
                if (gradeFilter && participant.grade !== gradeFilter) return;
                
                if (!teamStats[participant.team]) {
                    teamStats[participant.team] = {
                        team: participant.team,
                        daesang: 0,
                        gold: 0,
                        silver: 0,
                        bronze: 0,
                        total: 0
                    };
                }
                
                const participantResults = results.filter(r => r.participantId === participant.id);
                
                teamStats[participant.team].daesang += participantResults.filter(r => r.award === '대상').length;
                teamStats[participant.team].gold += participantResults.filter(r => r.award === '금상').length;
                teamStats[participant.team].silver += participantResults.filter(r => r.award === '은상').length;
                teamStats[participant.team].bronze += participantResults.filter(r => r.award === '동상').length;
            });
            
            // 총점 계산 및 정렬
            const sortedStats = Object.values(teamStats)
                .map(stat => {
                    stat.total = stat.daesang * 4 + stat.gold * 3 + stat.silver * 2 + stat.bronze;
                    return stat;
                })
                .filter(stat => stat.total > 0)
                .sort((a, b) => b.total - a.total);
            
            const rankingsHtml = sortedStats.map((stat, index) => `
                <tr>
                    <td>${index + 1}</td>
                    <td>${stat.team}</td>
                    <td>${stat.daesang}</td>
                    <td>${stat.gold}</td>
                    <td>${stat.silver}</td>
                    <td>${stat.bronze}</td>
                    <td>${stat.total}</td>
                </tr>
            `).join('');
            
            teamRankings.innerHTML = rankingsHtml || '<tr><td colspan="7">단체 순위 데이터가 없습니다.</td></tr>';
        }
        
        // 시상 기준 로드
        function loadCriteria() {
            const criteriaList = document.getElementById('criteriaList');
            const eventFilter = document.getElementById('criteriaFilterEvent').value;
            
            let criteriaHtml = '';
            
            for (const event in awardCriteria) {
                if (eventFilter && event !== eventFilter) continue;
                
                for (const grade in awardCriteria[event]) {
                    const criteria = awardCriteria[event][grade];
                    criteriaHtml += `
                        <tr>
                            <td>${event}</td>
                            <td>${grade}</td>
                            <td>${criteria.gold}</td>
                            <td>${criteria.silver}</td>
                            <td>${criteria.bronze}</td>
                            <td>
                                <button onclick="editCriteria('${event}', '${grade}')" class="info">수정</button>
                                <button onclick="deleteCriteria('${event}', '${grade}')" class="danger">삭제</button>
                            </td>
                        </tr>
                    `;
                }
            }
            
            criteriaList.innerHTML = criteriaHtml || '<tr><td colspan="6">등록된 시상 기준이 없습니다.</td></tr>';
        }
        
        // 시상 기준 추가/수정
        document.getElementById('criteriaForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const event = document.getElementById('criteriaEvent').value;
            const grade = document.getElementById('criteriaGrade').value;
            const gold = parseFloat(document.getElementById('criteriaGold').value);
            const silver = parseFloat(document.getElementById('criteriaSilver').value);
            const bronze = parseFloat(document.getElementById('criteriaBronze').value);
            
            // 기준 검증
            if (gold <= silver || silver <= bronze || bronze <= 0) {
                showNotification('시상 기준이 올바르지 않습니다. (금상 > 은상 > 동상 > 0)', 'error');
                return;
            }
            
            // awardCriteria 구조 초기화
            if (!awardCriteria[event]) {
                awardCriteria[event] = {};
            }
            
            // 시상 기준 저장
            awardCriteria[event][grade] = { gold, silver, bronze };
            localStorage.setItem('awardCriteria', JSON.stringify(awardCriteria));
            
            showNotification('시상 기준이 저장되었습니다.', 'success');
            loadCriteria();
            
            // 폼 초기화
            document.getElementById('criteriaForm').reset();
        });
        
        // 시상 기준 수정
        function editCriteria(event, grade) {
            const criteria = awardCriteria[event][grade];
            
            document.getElementById('criteriaEvent').value = event;
            document.getElementById('criteriaGrade').value = grade;
            document.getElementById('criteriaGold').value = criteria.gold;
            document.getElementById('criteriaSilver').value = criteria.silver;
            document.getElementById('criteriaBronze').value = criteria.bronze;
            
            // 스크롤 이동
            document.getElementById('criteriaForm').scrollIntoView();
        }
        
        // 시상 기준 삭제
        function deleteCriteria(event, grade) {
            if (confirm('정말로 이 시상 기준을 삭제하시겠습니까?')) {
                delete awardCriteria[event][grade];
                
                // 해당 이벤트에 기준이 더 이상 없으면 이벤트 삭제
                if (Object.keys(awardCriteria[event]).length === 0) {
                    delete awardCriteria[event];
                }
                
                localStorage.setItem('awardCriteria', JSON.stringify(awardCriteria));
                showNotification('시상 기준이 삭제되었습니다.', 'success');
                loadCriteria();
            }
        }
        
        // 사용자 로드
        function loadUsers() {
            if (currentUser.role !== 'admin') return;
            
            const usersList = document.getElementById('usersList');
            
            const usersHtml = users.map(user => `
                <tr>
                    <td>${user.username}</td>
                    <td>${user.role === 'admin' ? '관리자' : '기록 담당자(심판)'}</td>
                    <td>
                        <button onclick="editUser('${user.username}')" class="info">수정</button>
                        ${user.username !== currentUser.username ? 
                            `<button onclick="deleteUser('${user.username}')" class="danger">삭제</button>` : 
                            ''}
                    </td>
                </tr>
            `).join('');
            
            usersList.innerHTML = usersHtml || '<tr><td colspan="3">등록된 사용자가 없습니다.</td></tr>';
        }
        
        // 사용자 추가
        document.getElementById('userForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const username = document.getElementById('newUsername').value;
            const password = document.getElementById('newPassword').value;
            const role = document.getElementById('newUserRole').value;
            
            // 중복 사용자명 확인
            if (users.some(u => u.username === username)) {
                showNotification('이미 존재하는 사용자명입니다.', 'error');
                return;
            }
            
            users.push({ username, password, role });
            localStorage.setItem('users', JSON.stringify(users));
            
            showNotification('사용자가 성공적으로 추가되었습니다.', 'success');
            loadUsers();
            
            // 폼 초기화
            document.getElementById('userForm').reset();
        });
        
        // 사용자 수정
        function editUser(username) {
            const user = users.find(u => u.username === username);
            if (!user) return;
            
            editingUser = username;
            
            document.getElementById('editUsername').value = user.username;
            document.getElementById('editPassword').value = '';
            document.getElementById('editUserRole').value = user.role;
            
            document.getElementById('userEditForm').style.display = 'block';
            
            // 스크롤 이동
            document.getElementById('userEditForm').scrollIntoView();
        }
        
        // 사용자 수정 취소
        function cancelEditUser() {
            editingUser = null;
            document.getElementById('userEditForm').style.display = 'none';
            document.getElementById('editUserForm').reset();
        }
        
        // 사용자 수정 저장
        document.getElementById('editUserForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const username = document.getElementById('editUsername').value;
            const password = document.getElementById('editPassword').value;
            const role = document.getElementById('editUserRole').value;
            
            const userIndex = users.findIndex(u => u.username === editingUser);
            
            if (userIndex !== -1) {
                users[userIndex].role = role;
                
                // 비밀번호가 입력된 경우에만 업데이트
                if (password) {
                    users[userIndex].password = password;
                }
                
                localStorage.setItem('users', JSON.stringify(users));
                
                showNotification('사용자 정보가 수정되었습니다.', 'success');
                loadUsers();
                cancelEditUser();
            }
        });
        
        // 사용자 삭제
        function deleteUser(username) {
            if (username === currentUser.username) {
                showNotification('현재 로그인한 사용자는 삭제할 수 없습니다.', 'error');
                return;
            }
            
            if (confirm('정말로 이 사용자를 삭제하시겠습니까?')) {
                users = users.filter(u => u.username !== username);
                localStorage.setItem('users', JSON.stringify(users));
                
                showNotification('사용자가 삭제되었습니다.', 'success');
                loadUsers();
            }
        }
        
        // 엑셀 미리보기
        function previewExcel() {
            const fileInput = document.getElementById('excelFile');
            const file = fileInput.files[0];
            
            if (!file) {
                showNotification('엑셀 파일을 선택해주세요.', 'error');
                return;
            }
            
            const reader = new FileReader();
            
            reader.onload = function(e) {
                const data = new Uint8Array(e.target.result);
                const workbook = XLSX.read(data, { type: 'array' });
                
                // 첫 번째 시트 사용
                const worksheet = workbook.Sheets[workbook.SheetNames[0]];
                excelData = XLSX.utils.sheet_to_json(worksheet, { header: 1 });
                
                // 헤더 행 제거 (첫 번째 행)
                const headers = excelData.shift();
                
                // 미리보기 표시
                const previewBody = document.getElementById('previewBody');
                let previewHtml = '';
                
                for (let i = 0; i < Math.min(excelData.length, 10); i++) {
                    const row = excelData[i];
                    previewHtml += `
                        <tr>
                            <td>${row[0] || ''}</td>
                            <td>${row[1] || ''}</td>
                            <td>${row[2] || ''}</td>
                            <td>${row[3] || ''}</td>
                            <td>${validateParticipantData(row) ? '유효' : '오류'}</td>
                        </tr>
                    `;
                }
                
                previewBody.innerHTML = previewHtml;
                document.getElementById('excelPreview').style.display = 'block';
                document.getElementById('importBtn').style.display = 'block';
                
                if (excelData.length > 10) {
                    previewBody.innerHTML += `<tr><td colspan="5">...외 ${excelData.length - 10}행</td></tr>`;
                }
            };
            
            reader.readAsArrayBuffer(file);
        }
        
        // 참가자 데이터 유효성 검사
        function validateParticipantData(row) {
            if (row.length < 4) return false;
            if (!row[0] || !row[1] || !row[2] || !row[3]) return false;
            
            const validGrades = ['유치부', '초등1부', '초등2부', '초등3부', '초등4부', '초등5부', '초등6부', '중등부', '고등부', '일반부', '선수'];
            return validGrades.includes(row[3]);
        }
        
        // 엑셀 데이터 일괄 등록
        function importExcel() {
            if (excelData.length === 0) {
                showNotification('등록할 데이터가 없습니다.', 'error');
                return;
            }
            
            let successCount = 0;
            let errorCount = 0;
            let errorMessages = [];
            
            excelData.forEach((row, index) => {
                if (validateParticipantData(row)) {
                    const [id, name, team, grade] = row;
                    
                    // 중복 ID 확인
                    if (participants.some(p => p.id === id)) {
                        errorCount++;
                        errorMessages.push(`${index + 2}행: 중복된 참가자 번호 (${id})`);
                        return;
                    }
                    
                    participants.push({ id, name, team, grade });
                    successCount++;
                } else {
                    errorCount++;
                    errorMessages.push(`${index + 2}행: 데이터 형식 오류`);
                }
            });
            
            localStorage.setItem('participants', JSON.stringify(participants));
            
            // 결과 모달 표시
            const modalBody = document.getElementById('modalBody');
            modalBody.innerHTML = `
                <p>총 ${excelData.length}건 중 ${successCount}건 성공, ${errorCount}건 실패</p>
                ${errorMessages.length > 0 ? `
                    <p>오류 내용:</p>
                    <ul>
                        ${errorMessages.map(msg => `<li>${msg}</li>`).join('')}
                    </ul>
                ` : ''}
            `;
            
            document.getElementById('importModal').style.display = 'flex';
            
            // 데이터 갱신
            loadParticipants();
            updateDashboard();
            
            // 미리보기 초기화
            document.getElementById('excelPreview').style.display = 'none';
            document.getElementById('importBtn').style.display = 'none';
            document.getElementById('excelFile').value = '';
            excelData = [];
        }
        
        // 엑셀 템플릿 다운로드
        function downloadTemplate() {
            // 템플릿 데이터 생성
            const templateData = [
                ['번호', '이름', '소속', '참가부'],
                ['1001', '홍길동', '서울초등학교', '초등1부'],
                ['1002', '김철수', '서울초등학교', '초등2부'],
                ['1003', '이영희', '부산초등학교', '초등3부']
            ];
            
            // 워크북 생성
            const wb = XLSX.utils.book_new();
            const ws = XLSX.utils.aoa_to_sheet(templateData);
            
            // 컬럼 너비 설정
            const colWidths = [
                { wch: 10 }, // 번호
                { wch: 15 }, // 이름
                { wch: 20 }, // 소속
                { wch: 15 }  // 참가부
            ];
            ws['!cols'] = colWidths;
            
            // 워크북에 시트 추가
            XLSX.utils.book_append_sheet(wb, ws, '참가자템플릿');
            
            // 파일 다운로드
            XLSX.writeFile(wb, '줄넘기대회_참가자_템플릿.xlsx');
        }
        
        // 모달 닫기
        function closeModal() {
            document.getElementById('importModal').style.display = 'none';
        }
        
        // 알림 표시
        function showNotification(message, type) {
            const notification = document.getElementById('notification');
            notification.textContent = message;
            notification.className = `notification ${type}`;
            notification.style.display = 'block';
            
            setTimeout(() => {
                notification.style.display = 'none';
            }, 3000);
        }
        
        // 필터 변경 이벤트
        document.getElementById('participantFilterTeam').addEventListener('input', loadParticipants);
        document.getElementById('participantFilterGrade').addEventListener('change', loadParticipants);
        document.getElementById('scoreFilterEvent').addEventListener('change', loadScores);
        document.getElementById('rankingFilter').addEventListener('change', loadRankings);
        document.getElementById('criteriaFilterEvent').addEventListener('change', loadCriteria);
        
        // 앱 초기화
        function initApp() {
            initializeData();
            
            // 모바일 감지
            if (/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent)) {
                document.body.classList.add('mobile-device');
                showNotification('모바일 최적화 모드로 실행됩니다.', 'info');
            }
            
            // 로그인 상태 확인
            const savedUser = localStorage.getItem('currentUser');
            if (savedUser) {
                currentUser = JSON.parse(savedUser);
                loadApp();
            }
        }
        
        // 앱 실행
        initApp();
    </script>
</body>
</html>
