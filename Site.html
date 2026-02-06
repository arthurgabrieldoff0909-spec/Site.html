<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Brasil Play Star - Dashboard</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        :root {
            --bg-body: #0a0b0d;
            --bg-card: #121317;
            --bg-input: #1a1b21;
            --primary-red: #e62e2e;
            --primary-blue: #47a7ff;
            --text-main: #ffffff;
            --text-dim: #9ca3af;
            --header-red: #d92b2b;
        }

        body {
            margin: 0; padding: 0;
            background-color: var(--bg-body);
            color: var(--text-main);
            font-family: 'Inter', -apple-system, sans-serif;
            overflow-x: hidden;
        }

        /* --- Header --- */
        .dash-header {
            background-color: var(--header-red);
            height: 50px;
            display: flex;
            align-items: center;
            justify-content: flex-end;
            padding: 0 15px;
            gap: 20px;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .dash-header i { font-size: 20px; cursor: pointer; color: white; }

        /* --- Sidebar --- */
        #sidebar {
            position: fixed;
            top: 0;
            right: -280px;
            width: 250px;
            height: 100%;
            background-color: var(--bg-card);
            z-index: 1100;
            transition: 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: -5px 0 25px rgba(0,0,0,0.8);
            padding: 20px;
            box-sizing: border-box;
        }

        #sidebar-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.7);
            z-index: 1050;
        }

        .sidebar-item {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 15px;
            border-radius: 8px;
            cursor: pointer;
            color: #ff4d4d;
            font-weight: bold;
            transition: 0.2s;
            margin-top: 20px;
        }

        .sidebar-item:hover { background: rgba(255, 77, 77, 0.1); }

        /* --- Layout --- */
        .container { width: 100%; max-width: 450px; margin: 0 auto; padding: 20px; box-sizing: border-box; }
        .form-section { display: none; }
        .active { display: block; }

        .logo-header { text-align: center; margin-bottom: 20px; }
        .logo-brasil { color: var(--primary-red); font-size: 24px; font-weight: 900; margin: 0; }
        .logo-star { font-size: 38px; font-weight: 900; font-style: italic; margin: -5px 0 0 0; }
        .logo-star span { color: var(--primary-blue); }

        .card { background-color: var(--bg-card); padding: 30px 20px; border-radius: 12px; position: relative; margin-bottom: 20px; }
        h2 { font-size: 24px; margin: 0 0 10px 0; }
        .link-toggle { color: var(--text-dim); font-size: 14px; margin-bottom: 25px; }
        .link-toggle span { color: white; cursor: pointer; font-weight: bold; }

        .form-group { margin-bottom: 15px; }
        label { display: block; font-size: 11px; font-weight: bold; margin-bottom: 5px; text-transform: uppercase; }
        
        input, textarea {
            width: 100%; background: var(--bg-input); border: none; padding: 14px;
            border-radius: 6px; color: white; box-sizing: border-box; outline: none;
            font-family: inherit;
        }

        .btn-submit {
            width: 100%; background: #1f2128; color: white; border: none;
            padding: 15px; border-radius: 50px; font-weight: bold; cursor: pointer; margin-top: 10px;
        }

        .btn-responder-gradient {
            width: 100%; height: 54px; margin-top: 25px; border: none; border-radius: 50px; 
            background: linear-gradient(90deg, #e62e2e 0%, #70588a 50%, #1da1f2 100%);
            color: white; font-size: 18px; font-weight: 600; cursor: pointer;
            display: flex; align-items: center; justify-content: center;
        }

        .replies-container { margin-top: 30px; border-top: 1px solid #333; padding-top: 20px; }
        .reply-item { background: #1a1b21; padding: 15px; border-radius: 8px; margin-bottom: 10px; border-left: 2px solid var(--primary-blue); }
        .reply-user { font-weight: bold; color: var(--primary-blue); font-size: 13px; margin-bottom: 5px; display: block; }
        .reply-text { font-size: 14px; color: #ddd; }

        .topic-item {
            background: var(--bg-card); border-left: 4px solid var(--primary-red);
            padding: 15px; border-radius: 6px; margin-bottom: 12px; cursor: pointer;
        }

        .topic-user-row { display: flex; align-items: center; gap: 8px; margin-bottom: 8px; }
        .avatar-small { width: 24px; height: 24px; background: #333; border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 10px; }
        .topic-username { font-size: 13px; font-weight: bold; color: var(--primary-blue); }
        .topic-title { font-weight: bold; font-size: 15px; margin-bottom: 4px; display: block; }
        .topic-content { font-size: 13px; color: var(--text-dim); line-height: 1.4; }

        #modal-create {
            display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.95); z-index: 1000; padding: 20px; box-sizing: border-box;
            overflow-y: auto;
        }
        .btn-publish {
            width: 100%; background: var(--primary-red); color: white; border: none;
            padding: 15px; border-radius: 8px; font-weight: bold; cursor: pointer; margin-top: 10px;
        }

        .topic-image-display { width: 100%; max-height: 300px; object-fit: cover; border-radius: 8px; margin: 15px 0; }
        
        .btn-delete-topic {
            float: right;
            color: #ff4d4d;
            cursor: pointer;
            font-size: 18px;
            transition: 0.2s;
        }
        .btn-delete-topic:hover { transform: scale(1.2); }
    </style>
</head>
<body>

    <div id="sidebar-overlay" onclick="toggleSidebar(false)"></div>

    <div id="sidebar">
        <div style="display: flex; justify-content: space-between; align-items: center;">
            <span style="font-weight: bold; color: var(--text-dim); display: flex; align-items: center;">
                OPÇÕES <i class="fa-solid fa-bell" style="color: white; margin-left: 15px;"></i>
            </span>
            <i class="fa-solid fa-xmark" onclick="toggleSidebar(false)" style="font-size: 22px; cursor: pointer;"></i>
        </div>
        
        <div class="sidebar-item" onclick="handleLogout()">
            <i class="fa-solid fa-right-from-bracket"></i>
            <span>Sair</span>
        </div>
    </div>

    <header class="dash-header" id="user-header" style="display: none;">
        <i class="fa-solid fa-plus" onclick="toggleModal(true)"></i>
        <i class="fa-solid fa-bars" onclick="toggleSidebar(true)"></i>
    </header>

    <div class="container">
        
        <header class="logo-header" id="main-logo">
            <h1 class="logo-brasil">BRASIL PLAY STAR</h1>
        </header>

        <div id="login-screen" class="form-section active">
            <div class="card">
                <h2>Entre</h2>
                <p class="link-toggle">Ainda não tem uma conta? <span onclick="showScreen('register-screen')">Cadastre-se</span></p>
                <div class="form-group"><label>E-mail</label><input type="email" id="login-email" placeholder="seu@email.com"></div>
                <div class="form-group"><label>Senha</label><input type="password" id="login-pass" placeholder="Digite sua senha"></div>
                <button class="btn-submit" onclick="handleLogin()">Entrar</button>
            </div>
        </div>

        <div id="register-screen" class="form-section">
            <div class="card">
                <h2>Criar Conta</h2>
                <p class="link-toggle">Já possui conta? <span onclick="showScreen('login-screen')">Fazer Login</span></p>
                <div class="form-group">
                    <label>Usuário (Mínimo 4 caracteres)</label>
                    <input type="text" id="reg-user" placeholder="Ex: Gaba">
                </div>
                <div class="form-group"><label>E-mail</label><input type="email" id="reg-email" placeholder="email@exemplo.com"></div>
                <div class="form-group"><label>Senha</label><input type="password" id="reg-pass" placeholder="******"></div>
                <button class="btn-submit" onclick="handleRegister()">Criar Conta</button>
            </div>
        </div>

        <div id="dashboard-screen" class="form-section">
            <div style="text-align: left; margin-bottom: 20px;">
                <h1 class="logo-brasil" style="font-size: 18px;">BRASIL</h1>
                <h1 class="logo-star" style="font-size: 26px;">PLAY <span>STAR</span></h1>
            </div>
            <div id="topics-list"></div>
        </div>

        <div id="view-screen" class="form-section">
            <div style="cursor:pointer; margin-bottom: 20px; color: var(--text-dim);" onclick="showScreen('dashboard-screen')">
                <i class="fa-solid fa-arrow-left"></i> Voltar
            </div>
            <div id="full-topic-display"></div>
            <div id="replies-area" class="replies-container">
                <div id="replies-list"></div>
                <div class="card" style="margin-top: 20px;">
                    <textarea id="reply-text-input" rows="3" placeholder="Escreva algo..."></textarea>
                    <button class="btn-responder-gradient" id="btn-enviar-resposta">Responder</button>
                </div>
            </div>
        </div>
    </div>

    <div id="modal-create">
        <div style="display:flex; justify-content: space-between; margin-bottom: 20px;">
            <span style="font-size: 20px; font-weight: bold;">Novo Tópico</span>
            <i class="fa-solid fa-xmark" onclick="toggleModal(false)" style="font-size: 24px; cursor:pointer;"></i>
        </div>
        <div class="form-group"><label>Título</label><input type="text" id="topic-title-input"></div>
        <div class="form-group"><label>Conteúdo</label><textarea id="topic-content-input" rows="5"></textarea></div>
        <div class="form-group">
            <label>Provas abaixo (Opcional)</label>
            <input type="file" id="topic-image-input" accept="image/*">
        </div>
        <button class="btn-publish" onclick="publishTopic()">Publicar</button>
    </div>

    <script>
        // URL DO SEU FIREBASE
        const DATABASE_URL = "https://site-971eb-default-rtdb.firebaseio.com";
        
        let currentUser = null;
        let activeTopicId = null;

        // --- FUNÇÕES DE BANCO DE DADOS (FIREBASE) ---
        async function fbGet(path) {
            const res = await fetch(`${DATABASE_URL}${path}.json`);
            return await res.json();
        }

        async function fbPost(path, data) {
            await fetch(`${DATABASE_URL}${path}.json`, { method: 'POST', body: JSON.stringify(data) });
        }

        async function fbPut(path, data) {
            await fetch(`${DATABASE_URL}${path}.json`, { method: 'PUT', body: JSON.stringify(data) });
        }

        async function fbDelete(path) {
            await fetch(`${DATABASE_URL}${path}.json`, { method: 'DELETE' });
        }

        // --- INTERFACE ---
        function toggleSidebar(open) {
            const sidebar = document.getElementById('sidebar');
            const overlay = document.getElementById('sidebar-overlay');
            sidebar.style.right = open ? "0px" : "-280px";
            overlay.style.display = open ? "block" : "none";
        }

        function showScreen(id) {
            document.querySelectorAll('.form-section').forEach(s => s.classList.remove('active'));
            document.getElementById(id).classList.add('active');
            const header = document.getElementById('user-header');
            const mainLogo = document.getElementById('main-logo');
            
            if(id === 'dashboard-screen' || id === 'view-screen') {
                header.style.display = 'flex';
                mainLogo.style.display = 'none';
                if(id === 'dashboard-screen') loadTopics();
            } else {
                header.style.display = 'none';
                mainLogo.style.display = 'block';
            }
        }

        function handleLogout() {
            currentUser = null;
            toggleSidebar(false);
            showScreen('login-screen');
        }

        // --- AUTH ---
        async function handleRegister() {
            const user = document.getElementById('reg-user').value.trim();
            const emailRaw = document.getElementById('reg-email').value.trim();
            const emailKey = emailRaw.replace(/\./g, ','); // Firebase não aceita "." em chaves
            const pass = document.getElementById('reg-pass').value;

            if(!user || !emailRaw || !pass) return alert("Preencha tudo!");
            
            const users = await fbGet('/users') || {};
            if(users[emailKey]) return alert("E-mail já existe!");

            await fbPut(`/users/${emailKey}`, { user, pass, email: emailRaw });
            alert("Conta criada!");
            showScreen('login-screen');
        }

        async function handleLogin() {
            const emailKey = document.getElementById('login-email').value.trim().replace(/\./g, ',');
            const pass = document.getElementById('login-pass').value;
            
            const userData = await fbGet(`/users/${emailKey}`);
            if(userData && userData.pass === pass) {
                currentUser = userData;
                showScreen('dashboard-screen');
            } else {
                alert("Dados incorretos!");
            }
        }

        // --- TOPICOS ---
        function toggleModal(open) { 
            document.getElementById('modal-create').style.display = open ? 'block' : 'none'; 
        }

        async function publishTopic() {
            const title = document.getElementById('topic-title-input').value;
            const content = document.getElementById('topic-content-input').value;
            const imageFile = document.getElementById('topic-image-input').files[0];

            if(!title || !content) return alert("Preencha título e conteúdo!");

            if (imageFile) {
                const reader = new FileReader();
                reader.onloadend = () => saveToFirebase(title, content, reader.result);
                reader.readAsDataURL(imageFile);
            } else {
                saveToFirebase(title, content, null);
            }
        }

        async function saveToFirebase(title, content, imageData) {
            const topic = {
                author: currentUser.user,
                title,
                content,
                image: imageData,
                date: new Date().toLocaleString(),
                timestamp: Date.now()
            };
            await fbPost('/topics', topic);
            toggleModal(false);
            loadTopics();
        }

        async function loadTopics() {
            const container = document.getElementById('topics-list');
            container.innerHTML = "Carregando...";
            const data = await fbGet('/topics');
            
            if(!data) {
                container.innerHTML = "Nenhum tópico.";
                return;
            }

            const list = Object.keys(data).map(key => ({ id: key, ...data[key] }));
            list.sort((a,b) => b.timestamp - a.timestamp);

            container.innerHTML = list.map(t => `
                <div class="topic-item" onclick="viewTopic('${t.id}')">
                    <div class="topic-user-row">
                        <div class="avatar-small"><i class="fa-solid fa-user"></i></div>
                        <span class="topic-username">${t.author}</span>
                    </div>
                    <span class="topic-title">${t.title}</span>
                    <div class="topic-content">${t.content.substring(0, 60)}...</div>
                </div>
            `).join('');
        }

        async function viewTopic(id) {
            activeTopicId = id;
            const topic = await fbGet(`/topics/${id}`);
            if(!topic) return;

            const isOwner = currentUser && currentUser.user === topic.author;
            const deleteBtn = isOwner ? `<i class="fa-solid fa-trash-can btn-delete-topic" onclick="deleteTopic('${id}')"></i>` : '';

            document.getElementById('full-topic-display').innerHTML = `
                <div class="card">
                    ${deleteBtn}
                    <span class="topic-username">${topic.author}</span>
                    <h2 style="color: var(--primary-blue); margin-top: 10px;">${topic.title}</h2>
                    ${topic.image ? `<img src="${topic.image}" class="topic-image-display">` : ''}
                    <p style="white-space: pre-wrap; font-size: 15px; color: #eee; line-height: 1.5;">${topic.content}</p>
                    <small style="color: var(--text-dim); font-size: 10px;">Postado em: ${topic.date}</small>
                </div>
            `;
            loadReplies(id);
            showScreen('view-screen');
        }

        async function deleteTopic(id) {
            if(confirm("Excluir tópico?")) {
                await fbDelete(`/topics/${id}`);
                await fbDelete(`/replies/${id}`);
                showScreen('dashboard-screen');
            }
        }

        // --- RESPOSTAS ---
        async function loadReplies(topicId) {
            const data = await fbGet(`/replies/${topicId}`);
            const list = document.getElementById('replies-list');
            if(!data) { list.innerHTML = ""; return; }

            list.innerHTML = Object.values(data).map(r => `
                <div class="reply-item">
                    <span class="reply-user">@${r.author}</span>
                    <div class="reply-text">${r.text}</div>
                </div>
            `).join('');
        }

        document.getElementById('btn-enviar-resposta').addEventListener('click', async () => {
            const text = document.getElementById('reply-text-input').value.trim();
            if(!text) return;

            await fbPost(`/replies/${activeTopicId}`, {
                author: currentUser.user,
                text: text,
                timestamp: Date.now()
            });
            document.getElementById('reply-text-input').value = "";
            loadReplies(activeTopicId);
        });
    </script>
</body>
</html>
