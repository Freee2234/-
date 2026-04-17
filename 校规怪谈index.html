<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>校规怪谈</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #000;
            color: #c0c0c0;
            font-family: "Microsoft YaHei", "SimSun", sans-serif;
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* 噪点效果 */
        .noise {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1000;
            opacity: 0.15;
            background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)'/%3E%3C/svg%3E");
        }

        /* 故障效果 */
        .glitch {
            animation: glitch 0.3s infinite;
        }

        @keyframes glitch {
            0% { transform: translate(0); filter: hue-rotate(0deg); }
            20% { transform: translate(-3px, 3px); filter: hue-rotate(90deg); }
            40% { transform: translate(3px, -3px); filter: hue-rotate(180deg); }
            60% { transform: translate(-3px, -3px); filter: hue-rotate(270deg); }
            80% { transform: translate(3px, 3px); filter: hue-rotate(360deg); }
            100% { transform: translate(0); filter: hue-rotate(0deg); }
        }

        /* 开始界面 */
        #startScreen {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            padding: 20px;
        }

        .title {
            font-size: 4rem;
            color: #d4af37;
            text-shadow: 0 0 30px rgba(212, 175, 55, 0.6);
            margin-bottom: 30px;
            letter-spacing: 10px;
            font-weight: bold;
        }

        .note {
            background: #f5f5dc;
            color: #333;
            padding: 35px;
            max-width: 500px;
            border-radius: 3px;
            font-family: "KaiTi", "STKaiti", serif;
            line-height: 2.2;
            font-size: 1.1rem;
            box-shadow: 0 10px 40px rgba(0,0,0,0.6);
            transform: rotate(-1deg);
        }

        .note .warning {
            color: #8b0000;
            font-weight: bold;
            font-size: 1.15rem;
        }

        .startBtn {
            margin-top: 40px;
            padding: 15px 50px;
            background: transparent;
            border: 2px solid #d4af37;
            color: #d4af37;
            font-size: 1.3rem;
            cursor: pointer;
            letter-spacing: 8px;
            transition: all 0.3s;
        }

        .startBtn:hover {
            background: #d4af37;
            color: #000;
        }

        /* 游戏界面 */
        #gameScreen {
            display: none;
            min-height: 100vh;
        }

        /* 状态栏 */
        .statusBar {
            background: #0a0a0a;
            border-bottom: 2px solid #d4af37;
            padding: 15px 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 15px;
        }

        .statusItem {
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .gold {
            color: #d4af37;
        }

        .time {
            font-size: 1.8rem;
            color: #fff;
            font-family: "Courier New", monospace;
            font-weight: bold;
        }

        .sanityBox {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .sanityBar {
            width: 150px;
            height: 20px;
            background: #222;
            border-radius: 10px;
            overflow: hidden;
            border: 1px solid #444;
        }

        .sanityFill {
            height: 100%;
            background: linear-gradient(90deg, #228b22 0%, #d4af37 50%, #8b0000 100%);
            transition: width 0.3s ease;
        }

        /* 导航 */
        .nav {
            display: flex;
            justify-content: center;
            gap: 10px;
            padding: 15px;
            background: #050505;
            border-bottom: 1px solid #222;
            flex-wrap: wrap;
        }

        .navBtn {
            padding: 12px 30px;
            background: #1a1a1a;
            border: 1px solid #333;
            color: #666;
            cursor: pointer;
            font-size: 1rem;
            transition: all 0.3s;
        }

        .navBtn:hover {
            border-color: #d4af37;
            color: #d4af37;
        }

        .navBtn.active {
            background: #d4af37;
            color: #000;
            border-color: #d4af37;
        }

        /* 主体区域 */
        .main {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 20px;
            padding: 20px;
            max-width: 1400px;
            margin: 0 auto;
        }

        @media (max-width: 900px) {
            .main {
                grid-template-columns: 1fr;
            }
        }

        /* 场景区域 */
        .sceneBox {
            background: #0a0a0a;
            border: 1px solid #2a2a2a;
            border-radius: 5px;
            padding: 25px;
            min-height: 400px;
        }

        .sceneTitle {
            font-size: 2rem;
            color: #d4af37;
            margin-bottom: 15px;
            letter-spacing: 5px;
        }

        .sceneDesc {
            color: #999;
            line-height: 1.9;
            margin-bottom: 25px;
            font-size: 1.05rem;
        }

        .objects {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            margin-bottom: 20px;
        }

        .objBtn {
            padding: 12px 22px;
            background: #151515;
            border: 1px solid #3a3a3a;
            color: #888;
            cursor: pointer;
            transition: all 0.3s;
        }

        .objBtn:hover {
            border-color: #d4af37;
            color: #d4af37;
        }

        .actions {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
        }

        .actBtn {
            padding: 12px 25px;
            background: #1e1e1e;
            border: 1px solid #3a3a3a;
            color: #aaa;
            cursor: pointer;
            transition: all 0.3s;
        }

        .actBtn:hover {
            border-color: #d4af37;
            color: #d4af37;
        }

        /* 信息面板 */
        .infoPanel {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .rulesBox {
            background: #f5f5dc;
            color: #333;
            padding: 20px;
            border-radius: 3px;
            font-family: "KaiTi", "STKaiti", serif;
        }

        .rulesTitle {
            color: #8b0000;
            text-align: center;
            font-size: 1.3rem;
            margin-bottom: 15px;
            letter-spacing: 5px;
            font-weight: bold;
        }

        .rule {
            padding: 10px 12px;
            margin: 8px 0;
            border-left: 3px solid #8b4513;
            font-size: 0.95rem;
            line-height: 1.6;
            background: rgba(139, 69, 19, 0.05);
        }

        .broadcast {
            background: #050505;
            border: 1px solid #1a1a1a;
            padding: 15px;
            max-height: 280px;
            overflow-y: auto;
        }

        .broadcastTitle {
            color: #d4af37;
            font-size: 1.1rem;
            margin-bottom: 12px;
            letter-spacing: 3px;
        }

        .event {
            padding: 10px 12px;
            margin: 6px 0;
            border-left: 2px solid;
            font-size: 0.9rem;
            line-height: 1.5;
        }

        .event.normal { border-color: #444; color: #777; }
        .event.warn { border-color: #d4af37; color: #d4af37; }
        .event.danger { border-color: #8b0000; color: #c44; }
        .event.death { border-color: #f00; color: #f66; background: rgba(139,0,0,0.1); }

        /* 弹窗 */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.95);
            z-index: 2000;
            justify-content: center;
            align-items: center;
        }

        .modalBox {
            background: #0f0f0f;
            border: 2px solid #d4af37;
            padding: 35px;
            max-width: 450px;
            text-align: center;
        }

        .modalTitle {
            color: #d4af37;
            font-size: 1.5rem;
            margin-bottom: 20px;
        }

        .modalText {
            color: #aaa;
            line-height: 2;
            margin-bottom: 25px;
            font-size: 1.05rem;
        }

        .modalBtns {
            display: flex;
            gap: 15px;
            justify-content: center;
        }

        .modalBtn {
            padding: 12px 30px;
            background: #1a1a1a;
            border: 1px solid #444;
            color: #bbb;
            cursor: pointer;
        }

        .modalBtn:hover {
            border-color: #d4af37;
            color: #d4af37;
        }

        /* 结局画面 */
        .ending {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: #000;
            z-index: 3000;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 30px;
        }

        .endTitle {
            font-size: 3rem;
            margin-bottom: 30px;
            letter-spacing: 10px;
        }

        .endTitle.good { color: #4f4; }
        .endTitle.bad { color: #f44; }
        .endTitle.secret { color: #a4f; }

        .endText {
            color: #888;
            max-width: 600px;
            line-height: 2.2;
            font-size: 1.1rem;
            margin-bottom: 40px;
        }

        .restartBtn {
            padding: 15px 50px;
            background: transparent;
            border: 2px solid #d4af37;
            color: #d4af37;
            font-size: 1.2rem;
            cursor: pointer;
            letter-spacing: 5px;
        }

        .restartBtn:hover {
            background: #d4af37;
            color: #000;
        }
    </style>
</head>
<body>
    <!-- 噪点层 -->
    <div class="noise"></div>

    <!-- 开始界面 -->
    <div id="startScreen">
        <h1 class="title">校规怪谈</h1>
        <div class="note">
            <p>同学们，学校封闭管理7天。</p>
            <p class="warning">
                不要数班级人数。<br>
                如果看到另一个自己，假装没看见。<br>
                食堂阿姨只有一张嘴，没有脸。
            </p>
            <p>记住，学校永远保护学生。</p>
        </div>
        <button class="startBtn" onclick="startGame()">进入校园</button>
    </div>

    <!-- 游戏界面 -->
    <div id="gameScreen">
        <!-- 状态栏 -->
        <div class="statusBar">
            <div class="statusItem">第 <span class="gold" id="dayDisplay">1</span> 天</div>
            <div class="time" id="timeDisplay">06:00</div>
            <div class="statusItem">存活: <span class="gold" id="survivorDisplay">60</span>人</div>
            <div class="sanityBox">
                <span>理智</span>
                <div class="sanityBar">
                    <div class="sanityFill" id="sanityFill" style="width: 100%"></div>
                </div>
                <span id="sanityNum">100</span>
            </div>
        </div>

        <!-- 导航 -->
        <div class="nav">
            <button class="navBtn active" data-room="classroom" onclick="goRoom('classroom')">教室</button>
            <button class="navBtn" data-room="corridor" onclick="goRoom('corridor')">走廊</button>
            <button class="navBtn" data-room="canteen" onclick="goRoom('canteen')">食堂</button>
            <button class="navBtn" data-room="dorm" onclick="goRoom('dorm')">宿舍</button>
        </div>

        <!-- 主体 -->
        <div class="main">
            <!-- 场景 -->
            <div class="sceneBox">
                <h2 class="sceneTitle" id="sceneName">教室</h2>
                <p class="sceneDesc" id="sceneDesc">清晨的教室，阳光无法照亮所有角落。课桌整齐排列，黑板上留着昨天的板书，时钟停在3:33。</p>
                <div class="objects" id="objectsBox"></div>
                <div class="actions" id="actionsBox"></div>
            </div>

            <!-- 信息面板 -->
            <div class="infoPanel">
                <!-- 学生守则 -->
                <div class="rulesBox">
                    <div class="rulesTitle">学生守则</div>
                    <div id="rulesList"></div>
                </div>
                <!-- 校园广播 -->
                <div class="broadcast">
                    <div class="broadcastTitle">校园广播</div>
                    <div id="eventList"></div>
                </div>
            </div>
        </div>
    </div>

    <!-- 弹窗 -->
    <div class="modal" id="modal">
        <div class="modalBox">
            <h3 class="modalTitle" id="modalTitle">提示</h3>
            <p class="modalText" id="modalText">内容</p>
            <div class="modalBtns" id="modalBtns"></div>
        </div>
    </div>

    <!-- 结局 -->
    <div class="ending" id="ending">
        <h2 class="endTitle" id="endTitle">结局</h2>
        <p class="endText" id="endText">描述</p>
        <button class="restartBtn" onclick="location.reload()">重新开始</button>
    </div>

    <script>
        // 游戏状态
        const gameState = {
            day: 1,
            time: 360, // 6:00 = 360分钟
            sanity: 100,
            survivors: 60,
            currentRoom: 'classroom',
            gameOver: false,
            deadStudents: [],
            revealedRules: 0
        };

        const studentNames = ['李明','王芳','张伟','刘洋','陈静','杨帆','赵磊','黄婷','周杰','吴倩','郑凯','孙丽','钱伟','何敏','林涛'];

        // 场景数据
        const rooms = {
            classroom: {
                name: '教室',
                desc: '清晨的教室，阳光无法照亮所有角落。课桌整齐排列，黑板上留着昨天的板书，时钟停在3:33。',
                objects: [
                    { name: '课桌', action: checkDesk },
                    { name: '黑板', action: checkBlackboard },
                    { name: '时钟', action: checkClock },
                    { name: '毕业照', action: checkPhoto }
                ],
                actions: [
                    { name: '数人数', action: countPeople },
                    { name: '上课', action: attendClass }
                ]
            },
            corridor: {
                name: '走廊',
                desc: '声控灯忽明忽暗，脚步声在空旷中回荡。两侧教室门紧闭，尽头有一面镜子。',
                objects: [
                    { name: '镜子', action: checkMirror },
                    { name: '储物柜', action: checkLocker },
                    { name: '窗户', action: checkWindow }
                ],
                actions: [
                    { name: '快速通过', action: passQuickly },
                    { name: '停留观察', action: stayObserve }
                ]
            },
            canteen: {
                name: '食堂',
                desc: '油腻的气味弥漫在空气中。打饭窗口后，阿姨背对着你，后脑勺上有一张嘴在微笑。',
                objects: [
                    { name: '阿姨', action: talkToAunt },
                    { name: '菜单', action: checkMenu },
                    { name: '食物', action: eatFood }
                ],
                actions: [
                    { name: '找座位', action: findSeat },
                    { name: '立即离开', action: () => goRoom('corridor') }
                ]
            },
            dorm: {
                name: '宿舍',
                desc: '霉味弥漫，室友的床鼓起人形。镜子被黑布遮盖，窗外传来诡异的校歌声。',
                objects: [
                    { name: '镜子', action: checkDormMirror },
                    { name: '室友的床', action: checkRoommate },
                    { name: '窗户', action: checkDormWindow }
                ],
                actions: [
                    { name: '睡觉', action: goSleep },
                    { name: '躲床底', action: hideUnderBed }
                ]
            }
        };

        // 规则列表
        const allRules = [
            '每天早晨6点必须到达教室',
            '时钟走动时闭眼数到十',
            '黑板出现红字立刻离开',
            '不要数班级人数',
            '食堂阿姨只有嘴没有脸',
            '夜间不要照镜子',
            '看到另一个自己假装没看见',
            '听到校歌不要跟着唱'
        ];

        let gameTimer, deathTimer;

        // 开始游戏
        function startGame() {
            document.getElementById('startScreen').style.display = 'none';
            document.getElementById('gameScreen').style.display = 'block';
            
            renderScene();
            updateRules();
            addEvent('封闭管理开始，60名学生被困学校', 'normal');
            
            // 时间流逝
            gameTimer = setInterval(() => {
                if (gameState.gameOver) return;
                
                gameState.time += 5;
                if (gameState.time >= 1440) {
                    gameState.time = 360;
                    nextDay();
                }
                
                updateDisplay();
                
                // 随机事件
                if (Math.random() < 0.08) randomEvent();
                
                // 理智低触发故障
                if (gameState.sanity <= 30) {
                    document.body.classList.add('glitch');
                } else {
                    document.body.classList.remove('glitch');
                }
            }, 2000);
            
            // 随机死亡
            deathTimer = setTimeout(randomDeath, 25000);
        }

        // 进入下一天
        function nextDay() {
            gameState.day++;
            if (gameState.day <= 7) {
                updateRules();
                addEvent(`第${gameState.day}天，新的学生守则已发布`, 'warn');
            }
            if (gameState.day > 7) {
                checkEnding();
            }
        }

        // 更新显示
        function updateDisplay() {
            const hours = Math.floor(gameState.time / 60);
            const mins = gameState.time % 60;
            document.getElementById('timeDisplay').textContent = 
                `${hours.toString().padStart(2,'0')}:${mins.toString().padStart(2,'0')}`;
            document.getElementById('dayDisplay').textContent = gameState.day;
            document.getElementById('survivorDisplay').textContent = gameState.survivors;
            document.getElementById('sanityFill').style.width = gameState.sanity + '%';
            document.getElementById('sanityNum').textContent = gameState.sanity;
        }

        // 更新规则
        function updateRules() {
            const list = document.getElementById('rulesList');
            list.innerHTML = '';
            const showCount = Math.min(gameState.day + 2, allRules.length);
            for (let i = 0; i < showCount; i++) {
                const div = document.createElement('div');
                div.className = 'rule';
                div.textContent = `【规则${i+1}】${allRules[i]}`;
                list.appendChild(div);
            }
        }

        // 切换场景
        function goRoom(roomId) {
            gameState.currentRoom = roomId;
            
            // 更新导航按钮
            document.querySelectorAll('.navBtn').forEach(btn => {
                btn.classList.remove('active');
                if (btn.dataset.room === roomId) btn.classList.add('active');
            });
            
            renderScene();
            addEvent(`进入${rooms[roomId].name}`, 'normal');
        }

        // 渲染场景
        function renderScene() {
            const room = rooms[gameState.currentRoom];
            document.getElementById('sceneName').textContent = room.name;
            document.getElementById('sceneDesc').textContent = room.desc;
            
            // 物体按钮
            const objBox = document.getElementById('objectsBox');
            objBox.innerHTML = '';
            room.objects.forEach(obj => {
                const btn = document.createElement('button');
                btn.className = 'objBtn';
                btn.textContent = obj.name;
                btn.onclick = obj.action;
                objBox.appendChild(btn);
            });
            
            // 行动按钮
            const actBox = document.getElementById('actionsBox');
            actBox.innerHTML = '';
            room.actions.forEach(act => {
                const btn = document.createElement('button');
                btn.className = 'actBtn';
                btn.textContent = act.name;
                btn.onclick = act.action;
                actBox.appendChild(btn);
            });
        }

        // ========== 场景交互 ==========

        function checkDesk() {
            showModal('课桌', '桌肚里有一张泛黄的纸条，上面用红笔写着："救我，我在镜子里"', [
                { text: '扔掉纸条', action: () => { changeSanity(-5); closeModal(); } },
                { text: '塞回去', action: () => { changeSanity(-10); closeModal(); } }
            ]);
        }

        function checkBlackboard() {
            showModal('血字黑板', '黑板上用红字写着："还剩59人"。数字在跳动，最后停在你的学号上。', [
                { text: '立刻逃离', action: () => { changeSanity(-10); closeModal(); goRoom('corridor'); } },
                { text: '擦掉字迹', action: () => { changeSanity(-20); closeModal(); } }
            ]);
        }

        function checkClock() {
            addEvent('时钟的秒针在倒转', 'warn');
            changeSanity(-10);
        }

        function checkPhoto() {
            addEvent('毕业照里的你背对镜头，而你的背开始发凉', 'danger');
            changeSanity(-15);
        }

        function countPeople() {
            const count = Math.floor(Math.random() * 30) + 40;
            showModal('数人数', `你数出${count}人，但教室里只有几个身影。所有"人"都转向你，它们没有脸。`, [
                { text: '大喊"60人！"', action: () => { changeSanity(-15); closeModal(); } },
                { text: '逃跑', action: () => { changeSanity(-30); closeModal(); } }
            ]);
        }

        function attendClass() {
            addEvent('老师没有脸，只有一张嘴在讲课', 'danger');
            changeSanity(-10);
        }

        function checkMirror() {
            const hour = Math.floor(gameState.time / 60);
            if (hour >= 22 || hour < 6) {
                showModal('午夜镜子', '镜中的你没跟着动，它缓缓抬起手，指向你的身后...', [
                    { text: '打碎镜子', action: () => { changeSanity(-30); closeModal(); } },
                    { text: '闭眼转身', action: () => { changeSanity(-20); closeModal(); } }
                ]);
            } else {
                addEvent('镜中的你眼神有些不对劲', 'warn');
                changeSanity(-10);
            }
        }

        function checkLocker() {
            addEvent('储物柜里塞满了头发，还有一张你的学生证', 'danger');
            changeSanity(-15);
        }

        function checkWindow() {
            addEvent('窗玻璃上浮现一张和你一模一样的脸', 'danger');
            changeSanity(-20);
        }

        function passQuickly() {
            addEvent('你快步走过，但听到了两双脚步声', 'warn');
            changeSanity(-10);
        }

        function stayObserve() {
            addEvent('灯全灭了，有东西在靠近你的后颈', 'danger');
            changeSanity(-20);
        }

        function talkToAunt() {
            if (Math.random() < 0.5) {
                addEvent('阿姨后脑勺的嘴笑了："今天的菜很新鲜"', 'warn');
                changeSanity(-10);
            } else {
                addEvent('阿姨的嘴紧闭着，她在生气', 'danger');
                changeSanity(-15);
            }
        }

        function checkMenu() {
            addEvent('第三道菜的名字是你的名字', 'danger');
            changeSanity(-15);
        }

        function eatFood() {
            if (Math.random() < 0.6) {
                addEvent('食物味道怪异，你的手指变长了', 'danger');
                changeSanity(-15);
            } else {
                addEvent('咬到硬物，是牙齿——你的牙齿', 'death');
                changeSanity(-25);
            }
        }

        function findSeat() {
            addEvent('对面的餐具自己在动，像是有人正在用餐', 'warn');
            changeSanity(-10);
        }

        function checkDormMirror() {
            const hour = Math.floor(gameState.time / 60);
            if (hour >= 22) {
                showModal('午夜镜子', '镜中的你疯狂敲打镜面，裂纹渗出黑色液体，一只苍白的手正从裂缝中伸出...', [
                    { text: '打碎它', action: () => { changeSanity(-30); closeModal(); } },
                    { text: '盖上黑布', action: () => { changeSanity(-20); closeModal(); } }
                ]);
            } else {
                addEvent('镜中的你转身速度比你慢了一拍', 'warn');
                changeSanity(-15);
            }
        }

        function checkRoommate() {
            addEvent('被子里是校服包着一面镜子，镜中的人在尖叫', 'danger');
            changeSanity(-15);
        }

        function checkDormWindow() {
            addEvent('歌声从身后传来，而你正背对着窗户', 'danger');
            changeSanity(-20);
        }

        function goSleep() {
            if (Math.random() < 0.4) {
                addEvent('床是温热的，像是有人刚离开', 'warn');
                changeSanity(-15);
            } else {
                addEvent('你睡着了，梦见自己被困在镜子里，而镜外的"你"正在微笑', 'danger');
                changeSanity(-10);
            }
        }

        function hideUnderBed() {
            addEvent('床底满是指甲抓痕，还有一张今天的日期', 'danger');
            changeSanity(-10);
        }

        // ========== 系统功能 ==========

        function randomEvent() {
            const events = [
                { text: '灯突然熄灭，有指甲刮墙的声音', sanity: -15 },
                { text: '感觉有人在你耳边呼吸，但转头空无一人', sanity: -10 },
                { text: '地面渗出暗红色的液体，散发着铁锈味', sanity: -20 },
                { text: '你的影子没有跟着你的动作移动', sanity: -25 },
                { text: '听到自己的声音在走廊里说话', sanity: -20 },
                { text: '书本自动翻页，停在某一页——是你的名字', sanity: -15 }
            ];
            const e = events[Math.floor(Math.random() * events.length)];
            addEvent(e.text, 'danger');
            changeSanity(e.sanity);
        }

        function randomDeath() {
            if (gameState.survivors <= 1 || gameState.gameOver) return;
            
            const alive = studentNames.filter(n => !gameState.deadStudents.includes(n));
            const victim = alive[Math.floor(Math.random() * alive.length)] || '某同学';
            
            gameState.deadStudents.push(victim);
            gameState.survivors--;
            
            addEvent(`${victim}消失了，剩余${gameState.survivors}人`, 'death');
            
            if (gameState.survivors <= 1) {
                showEnding('bad', '全班覆灭', '你是最后一个幸存者。但身后传来和你一模一样的脚步声，越来越近...');
            } else {
                deathTimer = setTimeout(randomDeath, 20000 + Math.random() * 15000);
            }
        }

        function changeSanity(delta) {
            gameState.sanity = Math.max(0, Math.min(100, gameState.sanity + delta));
            updateDisplay();
            if (gameState.sanity <= 0) {
                showEnding('bad', '精神崩溃', '你的理智归零，成为了校园里游荡的"学生"之一，永远在寻找下一个玩伴...');
            }
        }

        function addEvent(text, type) {
            const list = document.getElementById('eventList');
            const div = document.createElement('div');
            div.className = `event ${type}`;
            const hours = Math.floor(gameState.time / 60);
            const mins = gameState.time % 60;
            div.textContent = `[${hours}:${mins.toString().padStart(2,'0')}] ${text}`;
            list.insertBefore(div, list.firstChild);
        }

        function showModal(title, text, buttons) {
            document.getElementById('modalTitle').textContent = title;
            document.getElementById('modalText').textContent = text;
            const btnBox = document.getElementById('modalBtns');
            btnBox.innerHTML = '';
            buttons.forEach(b => {
                const btn = document.createElement('button');
                btn.className = 'modalBtn';
                btn.textContent = b.text;
                btn.onclick = b.action;
                btnBox.appendChild(btn);
            });
            document.getElementById('modal').style.display = 'flex';
        }

        function closeModal() {
            document.getElementById('modal').style.display = 'none';
        }

        function checkEnding() {
            if (gameState.sanity >= 70 && gameState.survivors >= 30) {
                showEnding('good', '【好结局】黎明', '第7天黎明，校门缓缓打开。你走出校园，阳光洒在脸上。但那些规则已刻进骨髓，你再也分不清现实与怪谈的边界...');
            } else if (gameState.sanity >= 50) {
                showEnding('secret', '【隐藏结局】传承', '你活下来了，但代价是成为新的"教务处"。你在泛黄的纸条上写下规则，等待下一批学生...');
            } else {
                showEnding('bad', '【坏结局】沉沦', '你撑到了第7天，但你的影子留在了学校。走出去的只是一个空壳，而真正的你永远困在了镜子里...');
            }
        }

        function showEnding(type, title, text) {
            gameState.gameOver = true;
            clearInterval(gameTimer);
            clearTimeout(deathTimer);
            
            document.getElementById('endTitle').textContent = title;
            document.getElementById('endTitle').className = 'endTitle ' + type;
            document.getElementById('endText').textContent = text;
            document.getElementById('ending').style.display = 'flex';
        }
    </script>
</body>
</html>
