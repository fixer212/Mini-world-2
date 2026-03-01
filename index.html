<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
<title>Mini World Helper</title>
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }
body {
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
background: #f5f7fa;
color: #1c1e21;
min-height: 100vh;
display: flex;
flex-direction: column;
transition: background 0.3s, color 0.3s;
}
body.dark {
background: #0a0f1e;
color: #fff;
}
.app {
flex: 1;
display: flex;
flex-direction: column;
max-width: 600px;
margin: 0 auto;
width: 100%;
background: inherit;
}
.header {
display: flex;
justify-content: space-between;
align-items: center;
padding: 15px 20px;
border-bottom: 1px solid rgba(0,0,0,0.1);
background: inherit;
}
body.dark .header {
border-bottom-color: rgba(255,255,255,0.1);
}
.header h1 {
font-size: 24px;
font-weight: 700;
background: linear-gradient(135deg, #4f5bd5 0%, #6b77e5 100%);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
}
.admin-lock {
background: none;
border: none;
font-size: 1.8rem;
cursor: pointer;
color: inherit;
transition: transform 0.2s;
padding: 8px;
border-radius: 12px;
}
.admin-lock:hover {
transform: scale(1.1);
background: rgba(79, 91, 213, 0.1);
}
.loading-spinner {
display: inline-block;
width: 20px;
height: 20px;
border: 3px solid rgba(79, 91, 213, 0.2);
border-radius: 50%;
border-top-color: #4f5bd5;
animation: spin 0.8s linear infinite;
}
@keyframes spin {
to { transform: rotate(360deg); }
}
.page {
flex: 1;
padding: 20px;
display: none;
overflow-y: auto;
}
.page.active {
display: block;
}
.search-bar {
position: sticky;
top: 0;
background: inherit;
z-index: 100;
padding-bottom: 15px;
}
.search-input {
width: 100%;
padding: 12px 16px;
border-radius: 24px;
border: 1px solid rgba(0,0,0,0.1);
background: white;
font-size: 16px;
transition: all 0.2s;
box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}
body.dark .search-input {
background: #1e2332;
border-color: rgba(255,255,255,0.1);
color: white;
box-shadow: 0 2px 8px rgba(0,0,0,0.2);
}
.search-input::placeholder {
color: #999;
}
.search-input:focus {
outline: none;
border-color: #4f5bd5;
box-shadow: 0 0 0 3px rgba(79, 91, 213, 0.2);
}
.sort-controls {
display: flex;
gap: 10px;
margin-top: 12px;
padding: 0;
}
.sort-btn {
flex: 1;
padding: 10px 14px;
border-radius: 12px;
border: 1px solid rgba(0,0,0,0.1);
background: white;
cursor: pointer;
font-size: 13px;
font-weight: 500;
color: #666;
transition: all 0.3s ease;
display: flex;
align-items: center;
justify-content: center;
gap: 5px;
box-shadow: 0 2px 6px rgba(0,0,0,0.04);
}
body.dark .sort-btn {
background: #1e2332;
border-color: rgba(255,255,255,0.1);
color: #aaa;
}
.sort-btn:hover {
border-color: #4f5bd5;
transform: translateY(-2px);
box-shadow: 0 4px 12px rgba(79, 91, 213, 0.15);
}
.sort-btn.active {
background: linear-gradient(135deg, #4f5bd5 0%, #6b77e5 100%);
color: white;
border-color: #4f5bd5;
box-shadow: 0 4px 12px rgba(79, 91, 213, 0.3);
}
.nav-bar {
display: flex;
justify-content: space-around;
align-items: center;
padding: 8px 0;
background: rgba(255,255,255,0.9);
backdrop-filter: blur(10px);
border-top: 1px solid rgba(0,0,0,0.1);
}
body.dark .nav-bar {
background: rgba(20,25,40,0.9);
border-top-color: rgba(255,255,255,0.1);
}
.nav-btn {
flex: 1;
text-align: center;
padding: 8px 0;
border: none;
background: transparent;
font-size: 14px;
font-weight: 500;
color: #666;
cursor: pointer;
display: flex;
flex-direction: column;
align-items: center;
gap: 4px;
transition: all 0.2s;
border-radius: 12px;
margin: 0 4px;
}
body.dark .nav-btn { color: #aaa; }
.nav-btn:hover {
background: rgba(79, 91, 213, 0.1);
}
.nav-btn.active {
color: #4f5bd5;
background: rgba(79, 91, 213, 0.15);
}
.nav-btn .icon { font-size: 22px; }
.category-grid {
display: grid;
grid-template-columns: 1fr 1fr;
gap: 15px;
margin-top: 20px;
}
.category-card {
background: linear-gradient(135deg, #fff 0%, #f9fafb 100%);
border-radius: 24px;
padding: 28px 20px;
text-align: center;
box-shadow: 0 4px 15px rgba(0,0,0,0.06);
border: 2px solid rgba(0,0,0,0.04);
cursor: pointer;
transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
position: relative;
overflow: hidden;
}
.category-card::before {
content: '';
position: absolute;
top: 0;
left: -100%;
width: 100%;
height: 100%;
background: linear-gradient(135deg, #4f5bd5 0%, #6b77e5 100%);
opacity: 0;
transition: left 0.3s ease;
z-index: -1;
}
.category-card:hover {
transform: translateY(-8px);
box-shadow: 0 12px 30px rgba(79, 91, 213, 0.2);
border-color: #4f5bd5;
}
.category-card:hover::before {
left: 0;
opacity: 0.05;
}
body.dark .category-card {
background: linear-gradient(135deg, #1e2332 0%, #252d3d 100%);
border-color: rgba(255,255,255,0.08);
box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}
.category-card h3 {
font-size: 22px;
margin-bottom: 8px;
font-weight: 700;
background: linear-gradient(135deg, #4f5bd5 0%, #6b77e5 100%);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
transition: all 0.3s;
}
.category-card:hover h3 {
transform: scale(1.05);
}
.category-card p {
font-size: 14px;
color: #666;
font-weight: 500;
}
body.dark .category-card p {
color: #aaa;
}
.post-list { list-style: none; }
.post-item {
background: white;
border-radius: 16px;
padding: 16px;
margin-bottom: 12px;
border: 1px solid rgba(0,0,0,0.05);
cursor: pointer;
transition: all 0.3s ease;
box-shadow: 0 2px 8px rgba(0,0,0,0.04);
position: relative;
overflow: hidden;
}
.post-item::before {
content: '';
position: absolute;
left: 0;
top: 0;
width: 4px;
height: 100%;
background: linear-gradient(180deg, #4f5bd5 0%, #6b77e5 100%);
transform: scaleY(0);
transform-origin: center;
transition: transform 0.3s ease;
}
.post-item:hover {
transform: translateX(6px);
box-shadow: 0 8px 16px rgba(79, 91, 213, 0.12);
}
.post-item:hover::before {
transform: scaleY(1);
}
body.dark .post-item {
background: #1e2332;
border-color: rgba(255,255,255,0.08);
box-shadow: 0 2px 8px rgba(0,0,0,0.2);
}
.post-title { 
font-weight: 700; 
margin-bottom: 6px; 
font-size: 16px;
color: #1c1e21;
}
body.dark .post-title {
color: #fff;
}
.post-excerpt { 
font-size: 14px; 
color: #666;
line-height: 1.4;
}
body.dark .post-excerpt { 
color: #aaa; 
}
.post-date { 
font-size: 12px; 
color: #999; 
margin-top: 10px;
font-weight: 500;
}
body.dark .post-date { 
color: #777; 
}
.back-btn {
background: none;
border: none;
font-size: 16px;
margin-bottom: 20px;
color: #4f5bd5;
cursor: pointer;
display: flex;
align-items: center;
gap: 6px;
padding: 10px 14px;
border-radius: 30px;
transition: all 0.2s;
font-weight: 600;
}
.back-btn:hover {
background: rgba(79, 91, 213, 0.15);
transform: translateX(-4px);
}
.post-content {
background: white;
border-radius: 20px;
padding: 24px;
box-shadow: 0 4px 15px rgba(0,0,0,0.06);
}
body.dark .post-content { 
background: #1e2332;
box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}
.post-image {
max-width: 100%;
border-radius: 12px;
margin: 15px 0;
box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}
.code-block {
background: #f0f0f0;
border-radius: 12px;
padding: 15px;
font-family: 'Monaco', 'Menlo', monospace;
white-space: pre-wrap;
word-break: break-word;
margin: 15px 0;
border-left: 4px solid #4f5bd5;
font-size: 13px;
overflow-x: auto;
}
body.dark .code-block {
background: #2a2f40;
color: #e0e0e0;
border-left-color: #6b77e5;
}
.ai-explanation {
background: #e8f0fe;
border-radius: 18px;
padding: 16px;
margin: 20px 0 10px;
border-left: 4px solid #4f5bd5;
font-style: italic;
position: relative;
}
body.dark .ai-explanation {
background: #2a3150;
border-left-color: #8a96ff;
}
.ai-explanation::before {
content: "🤖 ИИ объясняет";
display: block;
font-weight: 600;
margin-bottom: 10px;
color: #4f5bd5;
font-style: normal;
}
body.dark .ai-explanation::before {
color: #8a96ff;
}
.ai-message {
background: #4f5bd5;
color: white;
padding: 12px 16px;
border-radius: 18px 18px 18px 4px;
max-width: 100%;
margin: 10px 0;
line-height: 1.5;
box-shadow: 0 2px 8px rgba(79, 91, 213, 0.3);
word-break: break-word;
}
body.dark .ai-message {
box-shadow: 0 2px 8px rgba(0,0,0,0.3);
}
.admin-panel {
background: white;
border-radius: 20px;
padding: 24px;
box-shadow: 0 4px 15px rgba(0,0,0,0.06);
}
body.dark .admin-panel { 
background: #1e2332;
box-shadow: 0 4px 15px rgba(0,0,0,0.3);
}
.admin-panel select, .admin-panel input, .admin-panel textarea {
width: 100%;
padding: 14px;
margin-bottom: 15px;
border-radius: 16px;
border: 1px solid #ddd;
font-size: 1rem;
transition: all 0.2s;
font-family: inherit;
}
.admin-panel select:focus, .admin-panel input:focus, .admin-panel textarea:focus {
outline: none;
border-color: #4f5bd5;
box-shadow: 0 0 0 3px rgba(79, 91, 213, 0.2);
}
body.dark .admin-panel select, body.dark .admin-panel input, body.dark .admin-panel textarea {
background: #2a2f40;
border-color: #444;
color: white;
}
.checkbox-field {
display: flex;
align-items: center;
gap: 10px;
margin-bottom: 20px;
padding: 12px 14px;
background: rgba(79, 91, 213, 0.08);
border-radius: 16px;
border: 1px solid rgba(79, 91, 213, 0.2);
cursor: pointer;
transition: all 0.2s;
}
.checkbox-field:hover {
background: rgba(79, 91, 213, 0.12);
}
.checkbox-field input[type="checkbox"] {
width: 20px;
height: 20px;
margin: 0;
accent-color: #4f5bd5;
cursor: pointer;
}
.checkbox-field label {
cursor: pointer;
font-weight: 500;
}
.btn {
background: linear-gradient(135deg, #4f5bd5 0%, #6b77e5 100%);
color: white;
border: none;
border-radius: 16px;
padding: 14px 24px;
font-size: 1rem;
font-weight: 600;
cursor: pointer;
transition: all 0.3s;
box-shadow: 0 4px 12px rgba(79, 91, 213, 0.3);
display: inline-flex;
align-items: center;
justify-content: center;
gap: 8px;
}
.btn:hover {
transform: translateY(-2px);
box-shadow: 0 6px 20px rgba(79, 91, 213, 0.4);
}
.btn:active {
transform: translateY(0);
}
.btn-danger {
background: linear-gradient(135deg, #d55f5f 0%, #e07070 100%);
box-shadow: 0 4px 12px rgba(213, 95, 95, 0.3);
}
.btn-danger:hover {
box-shadow: 0 6px 20px rgba(213, 95, 95, 0.4);
}
.btn-small {
padding: 8px 14px;
font-size: 13px;
}
.btn-group {
display: flex;
gap: 8px;
}
.btn-group .btn {
flex: 1;
padding: 10px 12px;
}
.admin-post-item {
display: flex;
justify-content: space-between;
align-items: center;
background: #f9f9f9;
border-radius: 16px;
padding: 14px;
margin-bottom: 10px;
border: 1px solid rgba(0,0,0,0.05);
transition: all 0.2s;
}
.admin-post-item:hover {
background: #f5f5f5;
box-shadow: 0 2px 8px rgba(0,0,0,0.06);
}
body.dark .admin-post-item { 
background: #2a2f40;
border-color: rgba(255,255,255,0.08);
}
body.dark .admin-post-item:hover {
background: #323a52;
}
.admin-post-title {
font-weight: 600;
color: #1c1e21;
flex: 1;
white-space: nowrap;
overflow: hidden;
text-overflow: ellipsis;
}
body.dark .admin-post-title {
color: #fff;
}
.modal {
position: fixed;
top: 0; left: 0; width: 100%; height: 100%;
background: rgba(0,0,0,0.5);
display: flex;
align-items: center;
justify-content: center;
z-index: 1000;
backdrop-filter: blur(5px);
}
.modal-content {
background: white;
padding: 28px;
border-radius: 24px;
max-width: 350px;
width: 90%;
box-shadow: 0 20px 40px rgba(0,0,0,0.2);
}
body.dark .modal-content { 
background: #1e2332;
box-shadow: 0 20px 40px rgba(0,0,0,0.4);
}
.modal-content h3 {
margin-bottom: 16px;
font-size: 18px;
font-weight: 700;
}
.password-input {
width: 100%;
padding: 14px;
border-radius: 16px;
border: 1px solid #ddd;
margin: 15px 0;
font-size: 16px;
transition: all 0.2s;
}
body.dark .password-input {
background: #2a2f40;
border-color: #444;
color: white;
}
.password-input:focus {
outline: none;
border-color: #4f5bd5;
box-shadow: 0 0 0 3px rgba(79, 91, 213, 0.2);
}
.remember-me {
display: flex;
align-items: center;
gap: 8px;
margin: 15px 0;
cursor: pointer;
}
.remember-me input {
cursor: pointer;
}
.settings-item {
background: white;
border-radius: 16px;
padding: 16px;
margin-bottom: 15px;
display: flex;
justify-content: space-between;
align-items: center;
box-shadow: 0 2px 8px rgba(0,0,0,0.04);
}
body.dark .settings-item { 
background: #1e2332;
box-shadow: 0 2px 8px rgba(0,0,0,0.2);
}
.switch {
position: relative;
display: inline-block;
width: 50px;
height: 24px;
}
.switch input { opacity: 0; width: 0; height: 0; }
.slider {
position: absolute;
cursor: pointer;
top: 0; left: 0; right: 0; bottom: 0;
background-color: #ccc;
transition: .3s;
border-radius: 24px;
}
.slider:before {
position: absolute;
content: "";
height: 20px;
width: 20px;
left: 2px;
bottom: 2px;
background-color: white;
transition: .3s;
border-radius: 50%;
}
input:checked + .slider { background: linear-gradient(135deg, #4f5bd5 0%, #6b77e5 100%); }
input:checked + .slider:before { transform: translateX(26px); }
.ai-input-area {
transition: all 0.3s ease;
overflow: hidden;
}
.ai-input-area.hidden {
display: none;
}
.empty-state {
text-align: center;
color: #999;
padding: 60px 20px;
}
.empty-state-icon {
font-size: 56px;
margin-bottom: 16px;
opacity: 0.8;
}
.empty-state p {
font-size: 16px;
color: #999;
}
body.dark .empty-state p {
color: #777;
}
.modal-buttons {
display: flex;
gap: 12px;
margin-top: 20px;
}
.modal-buttons .btn {
flex: 1;
}
.error-message {
background: #fee;
color: #c33;
padding: 12px 16px;
border-radius: 12px;
margin-bottom: 15px;
border-left: 4px solid #c33;
}
body.dark .error-message {
background: #3a2424;
color: #ff6b6b;
border-left-color: #ff6b6b;
}
.success-message {
background: #efe;
color: #3a3;
padding: 12px 16px;
border-radius: 12px;
margin-bottom: 15px;
border-left: 4px solid #3a3;
}
body.dark .success-message {
background: #243a24;
color: #6b6;
border-left-color: #6b6;
}
</style>
</head>
<body class="dark">
<div class="app">
<div class="header">
<h1>Mini World Helper</h1>
<button class="admin-lock" id="adminLockBtn" title="Админ-панель">🔒</button>
</div>

<!-- Страницы -->
<div id="homePage" class="page active">
<h2>Туториалы</h2>
<div class="category-grid">
<div class="category-card" data-category="triggers">
<h3>⚡ Триггеры</h3>
<p>События и условия</p>
</div>
<div class="category-card" data-category="scripts">
<h3>📝 Скрипты</h3>
<p>Примеры кода на Lua</p>
</div>
</div>
</div>

<div id="categoryPage" class="page">
<button class="back-btn" id="backFromCategory">← Назад</button>
<h2 id="categoryTitle"></h2>

<div id="loadingMessage" style="display: none; text-align: center; padding: 20px;">
<div class="loading-spinner"></div>
<p style="margin-top: 10px; color: #999;">Загрузка постов...</p>
</div>

<div id="errorMessage"></div>

<div class="search-bar">
<input type="text" id="searchInput" class="search-input" placeholder="🔍 Поиск постов...">
<div class="sort-controls">
<button class="sort-btn active" data-sort="newest" title="Самые новые посты">
<span>⬇️</span> <span>Новые</span>
</button>
<button class="sort-btn" data-sort="oldest" title="Самые старые посты">
<span>⬆️</span> <span>Старые</span>
</button>
<button class="sort-btn" data-sort="title" title="Сортировка по названию">
<span>🔤</span> <span>Название</span>
</button>
</div>
</div>

<div id="postList" class="post-list"></div>
</div>

<div id="postPage" class="page">
<button class="back-btn" id="backFromPost">← Назад</button>
<div id="postContent" class="post-content"></div>
</div>

<div id="adminPage" class="page">
<button class="back-btn" id="backFromAdmin">← Назад</button>
<h2>Админ-панель</h2>
<div id="adminErrorMessage"></div>
<div class="admin-panel">
<select id="adminCategory">
<option value="triggers">⚡ Триггеры</option>
<option value="scripts">📝 Скрипты</option>
</select>
<button class="btn" id="newPostBtn">➕ Новый пост</button>
<div id="adminPostList"></div>
</div>
</div>

<div id="adminEditPage" class="page">
<button class="back-btn" id="backFromEdit">← Назад</button>
<h2 id="editTitle">Создание поста</h2>
<div id="editErrorMessage"></div>
<div class="admin-panel">
<input type="text" id="postTitle" placeholder="Заголовок">
<textarea id="postText" placeholder="Основной текст поста" rows="6"></textarea>

<div id="scriptOptions" style="display: none;">
<div class="checkbox-field">
<input type="checkbox" id="aiEnabled">
<label for="aiEnabled">🤖 Добавить объяснение от ИИ</label>
</div>
<div id="aiInputArea" class="ai-input-area hidden">
<textarea id="aiExplanation" placeholder="Объяснение от ИИ (будет отформатировано автоматически)..." rows="5"></textarea>
</div>
<div id="codeField">
<textarea id="postCode" placeholder="Код на Lua" rows="8"></textarea>
</div>
</div>

<input type="file" id="postImage" accept="image/*">
<div id="imagePreview"></div>
<div class="btn-group">
<button class="btn" id="savePostBtn">💾 Сохранить</button>
<button class="btn btn-danger" id="deletePostBtn" style="display: none;">🗑️ Удалить</button>
</div>
</div>
</div>

<div id="settingsPage" class="page">
<h2>Настройки</h2>
<div class="settings-item">
<span>Тёмная тема</span>
<label class="switch">
<input type="checkbox" id="themeToggle" checked>
<span class="slider"></span>
</label>
</div>
</div>

<div id="chatPage" class="page">
<div class="empty-state">
<div class="empty-state-icon">💬</div>
<h3>Чат с ботом скоро появится</h3>
<p>Следите за обновлениями!</p>
</div>
</div>

<!-- Нижнее меню -->
<div class="nav-bar">
<button class="nav-btn" data-page="home"><span class="icon">🏠</span><span>Главная</span></button>
<button class="nav-btn" data-page="chat"><span class="icon">💬</span><span>Чат</span></button>
<button class="nav-btn" data-page="settings"><span class="icon">⚙️</span><span>Настройки</span></button>
</div>
</div>

<!-- Модалка пароля -->
<div id="passwordModal" class="modal" style="display: none;">
<div class="modal-content">
<h3>Введите пароль</h3>
<input type="password" id="passwordInput" class="password-input" placeholder="Пароль">
<div class="remember-me">
<input type="checkbox" id="rememberMe"> 
<label for="rememberMe">Запомнить меня</label>
</div>
<div class="modal-buttons">
<button class="btn" id="submitPassword">Войти</button>
<button class="btn btn-danger" id="cancelPassword">Отмена</button>
</div>
</div>
</div>

<!-- Модалка подтверждения удаления -->
<div id="deleteConfirmModal" class="modal" style="display: none;">
<div class="modal-content">
<h3>⚠️ Удалить пост?</h3>
<p style="color: #666; margin: 15px 0; line-height: 1.5;">Это действие невозможно будет отменить. Пост будет удалён безвозвратно.</p>
<div class="modal-buttons">
<button class="btn btn-danger" id="confirmDelete">🗑️ Удалить</button>
<button class="btn" id="cancelDelete">Отмена</button>
</div>
</div>
</div>

<script src="https://cdn.jsdelivr.net/npm/appwrite@latest"></script>

<script>
(function() {
// Appwrite конфигурация
const client = new Appwrite.Client();
client
  .setEndpoint('https://cloud.appwrite.io/v1')
  .setProject('69a1e6ea000bf85fe85e');

const database = new Appwrite.Databases(client);
const DB_ID = '69a1e85e001ee6e697e0';
const COLLECTION_ID = 'test';

let isDark = localStorage.getItem('theme') !== 'light';
let currentCategory = 'triggers';
let currentPostId = null;
let editingPost = null;
let currentSort = 'newest';
let currentSearch = '';
let pendingDeleteIndex = null;
let allPosts = [];

async function loadPostsFromAppwrite() {
try {
const response = await database.listDocuments(DB_ID, COLLECTION_ID);
allPosts = response.documents;
return allPosts;
} catch (error) {
console.error('Ошибка при загрузке постов:', error);
showError('errorMessage', 'Ошибка при загрузке данных с сервера');
return [];
}
}

async function createPost(data) {
try {
const doc = await database.createDocument(DB_ID, COLLECTION_ID, 'unique()', data);
return doc;
} catch (error) {
console.error('Ошибка при создании поста:', error);
showError('editErrorMessage', 'Ошибка при сохранении поста: ' + error.message);
throw error;
}
}

async function updatePost(docId, data) {
try {
const doc = await database.updateDocument(DB_ID, COLLECTION_ID, docId, data);
return doc;
} catch (error) {
console.error('Ошибка при обновлении поста:', error);
showError('editErrorMessage', 'Ошибка при сохранении поста: ' + error.message);
throw error;
}
}

async function deletePost(docId) {
try {
await database.deleteDocument(DB_ID, COLLECTION_ID, docId);
return true;
} catch (error) {
console.error('Ошибка при удалении поста:', error);
showError('adminErrorMessage', 'Ошибка при удалении поста: ' + error.message);
throw error;
}
}

function showError(elementId, message) {
const element = document.getElementById(elementId);
if (element) {
element.innerHTML = `<div class="error-message">${escapeHtml(message)}</div>`;
setTimeout(() => {
element.innerHTML = '';
}, 5000);
}
}

function showSuccess(message) {
alert(message);
}

// --- Элементы ---
const body = document.body;
const pages = document.querySelectorAll('.page');
const navBtns = document.querySelectorAll('.nav-btn');
const adminLock = document.getElementById('adminLockBtn');
const passwordModal = document.getElementById('passwordModal');
const passwordInput = document.getElementById('passwordInput');
const rememberMe = document.getElementById('rememberMe');
const submitPassword = document.getElementById('submitPassword');
const cancelPassword = document.getElementById('cancelPassword');
const themeToggle = document.getElementById('themeToggle');
const backFromCategory = document.getElementById('backFromCategory');
const backFromPost = document.getElementById('backFromPost');
const backFromAdmin = document.getElementById('backFromAdmin');
const backFromEdit = document.getElementById('backFromEdit');
const categoryTitle = document.getElementById('categoryTitle');
const postListDiv = document.getElementById('postList');
const postContentDiv = document.getElementById('postContent');
const adminCategory = document.getElementById('adminCategory');
const newPostBtn = document.getElementById('newPostBtn');
const adminPostList = document.getElementById('adminPostList');
const postTitle = document.getElementById('postTitle');
const postText = document.getElementById('postText');
const postCode = document.getElementById('postCode');
const postImage = document.getElementById('postImage');
const imagePreview = document.getElementById('imagePreview');
const savePostBtn = document.getElementById('savePostBtn');
const deletePostBtn = document.getElementById('deletePostBtn');
const scriptOptions = document.getElementById('scriptOptions');
const aiEnabled = document.getElementById('aiEnabled');
const aiExplanation = document.getElementById('aiExplanation');
const aiInputArea = document.getElementById('aiInputArea');
const searchInput = document.getElementById('searchInput');
const sortBtns = document.querySelectorAll('.sort-btn');
const deleteConfirmModal = document.getElementById('deleteConfirmModal');
const confirmDelete = document.getElementById('confirmDelete');
const cancelDelete = document.getElementById('cancelDelete');
const loadingMessage = document.getElementById('loadingMessage');

// --- Поиск и сортировка ---
searchInput.addEventListener('input', (e) => {
currentSearch = e.target.value.toLowerCase();
renderPostList();
});

sortBtns.forEach(btn => {
btn.addEventListener('click', () => {
sortBtns.forEach(b => b.classList.remove('active'));
btn.classList.add('active');
currentSort = btn.dataset.sort;
renderPostList();
});
});

function filterAndSortPosts(posts) {
let filtered = posts.filter(post => {
const category = post.test3 || '';
const searchText = currentSearch.toLowerCase();
return (
category.toLowerCase() === currentCategory &&
(
(post.title && post.title.toLowerCase().includes(searchText)) ||
(post.text && post.text.toLowerCase().includes(searchText))
)
);
});

filtered = filtered.map((post) => ({
...post,
timestamp: post.$createdAt ? new Date(post.$createdAt).getTime() : Date.now()
}));

switch(currentSort) {
case 'oldest':
filtered.sort((a, b) => a.timestamp - b.timestamp);
break;
case 'title':
filtered.sort((a, b) => (a.title || '').localeCompare(b.title || ''));
break;
case 'newest':
default:
filtered.sort((a, b) => b.timestamp - a.timestamp);
}

return filtered;
}

// --- Применение темы ---
function applyTheme() {
if (isDark) {
body.classList.add('dark');
themeToggle.checked = true;
} else {
body.classList.remove('dark');
themeToggle.checked = false;
}
localStorage.setItem('theme', isDark ? 'dark' : 'light');
}

// --- Переключение страниц ---
function showPage(pageId) {
pages.forEach(p => p.classList.remove('active'));
document.getElementById(pageId).classList.add('active');
navBtns.forEach(btn => {
const btnPage = btn.dataset.page;
btn.classList.toggle('active',
(btnPage === 'home' && pageId === 'homePage') ||
(btnPage === 'chat' && pageId === 'chatPage') ||
(btnPage === 'settings' && pageId === 'settingsPage')
);
});
}

navBtns.forEach(btn => {
btn.addEventListener('click', () => {
const page = btn.dataset.page;
currentSearch = '';
searchInput.value = '';
currentSort = 'newest';
showPage(page + 'Page');
});
});

// --- Главная: клик по категории ---
document.querySelectorAll('.category-card').forEach(card => {
card.addEventListener('click', async () => {
currentCategory = card.dataset.category;
categoryTitle.textContent = card.querySelector('h3').textContent;
currentSearch = '';
searchInput.value = '';
currentSort = 'newest';
document.querySelector('.sort-btn.active')?.classList.remove('active');
document.querySelector('[data-sort="newest"]').classList.add('active');
loadingMessage.style.display = 'block';
document.getElementById('errorMessage').innerHTML = '';
await loadPostsFromAppwrite();
renderPostList();
loadingMessage.style.display = 'none';
showPage('categoryPage');
});
});

function renderPostList() {
const filteredPosts = filterAndSortPosts(allPosts);

postListDiv.innerHTML = '';

if (filteredPosts.length === 0) {
if (currentSearch) {
postListDiv.innerHTML = `<div class="empty-state"><div class="empty-state-icon">🔍</div><p>Постов не найдено</p></div>`;
} else {
postListDiv.innerHTML = `<div class="empty-state"><div class="empty-state-icon">📭</div><p>Нет постов</p></div>`;
}
return;
}

filteredPosts.forEach((post) => {
const div = document.createElement('div');
div.className = 'post-item';
const postDate = new Date(post.$createdAt || Date.now());
const dateStr = postDate.toLocaleDateString('ru-RU');

let excerpt = post.text || '';
if (excerpt.length > 70) {
excerpt = excerpt.substring(0, 70) + '...';
}

div.innerHTML = `
<div class="post-title">${escapeHtml(post.title || 'Без названия')}</div>
<div class="post-excerpt">${escapeHtml(excerpt)}</div>
<div class="post-date">📅 ${dateStr}</div>
`;

div.addEventListener('click', () => {
currentPostId = post.$id;
renderPost();
showPage('postPage');
});

postListDiv.appendChild(div);
});
}

function renderPost() {
const post = allPosts.find(p => p.$id === currentPostId);

if (!post) return;

let html = `<h2>${escapeHtml(post.title || 'Без названия')}</h2>`;

const mainText = (post.text || '').trim();
if (mainText) {
html += `<p>${escapeHtml(mainText).replace(/\n/g, '<br>')}</p>`;
} else {
html += `<p style="color: #999; font-style: italic;">[Текст поста не заполнен]</p>`;
}

if (post.image) {
html += `<img src="${escapeHtml(post.image)}" class="post-image" alt="Изображение">`;
}

if (post.code && post.code.trim()) {
html += `<div style="margin-top: 20px;"><strong>📝 Код:</strong></div>`;
html += `<pre class="code-block">${escapeHtml(post.code)}</pre>`;
}

if (post.test2) {
const aiText = (post.test2 || '').trim();
if (aiText) {
html += `<div class="ai-explanation">`;
html += `<div class="ai-message">${escapeHtml(aiText).replace(/\n/g, '<br>')}</div>`;
html += `</div>`;
}
}

postContentDiv.innerHTML = html;
}

// --- Кнопки назад ---
backFromCategory.addEventListener('click', () => showPage('homePage'));
backFromPost.addEventListener('click', () => {
showPage('categoryPage');
renderPostList();
});
backFromAdmin.addEventListener('click', () => showPage('homePage'));
backFromEdit.addEventListener('click', () => {
showPage('adminPage');
renderAdminPostList();
});

// --- Управление отображением полей для скриптов ---
function updateScriptFields() {
const cat = adminCategory.value;
if (cat === 'scripts') {
scriptOptions.style.display = 'block';
if (aiEnabled.checked) {
aiInputArea.classList.remove('hidden');
} else {
aiInputArea.classList.add('hidden');
}
} else {
scriptOptions.style.display = 'none';
}
}

adminCategory.addEventListener('change', updateScriptFields);
aiEnabled.addEventListener('change', updateScriptFields);

// --- Админка ---
adminLock.addEventListener('click', () => {
if (localStorage.getItem('adminRemember') === 'true') {
showPage('adminPage');
renderAdminPostList();
} else {
passwordModal.style.display = 'flex';
}
});

cancelPassword.addEventListener('click', () => {
passwordModal.style.display = 'none';
passwordInput.value = '';
});

submitPassword.addEventListener('click', () => {
if (passwordInput.value === 'damoix001') {
if (rememberMe.checked) {
localStorage.setItem('adminRemember', 'true');
}
passwordModal.style.display = 'none';
passwordInput.value = '';
showPage('adminPage');
renderAdminPostList();
} else {
alert('Неверный пароль');
}
});

async function renderAdminPostList() {
const cat = adminCategory.value;
const categoryPosts = allPosts.filter(p => p.test3 === cat);
adminPostList.innerHTML = '';

if (categoryPosts.length === 0) {
adminPostList.innerHTML = '<p style="text-align:center; color:#999; padding: 20px;">Нет постов</p>';
return;
}

categoryPosts.forEach((post) => {
const div = document.createElement('div');
div.className = 'admin-post-item';
div.innerHTML = `
<span class="admin-post-title">${escapeHtml(post.title || 'Без названия')}</span>
<div class="btn-group">
<button class="btn btn-small" data-id="${post.$id}" data-action="edit">✏️</button>
<button class="btn btn-small btn-danger" data-id="${post.$id}" data-action="delete">🗑️</button>
</div>
`;
adminPostList.appendChild(div);
});

document.querySelectorAll('[data-action="edit"]').forEach(btn => {
btn.addEventListener('click', (e) => {
const docId = e.target.closest('button').dataset.id;
editPost(docId);
});
});

document.querySelectorAll('[data-action="delete"]').forEach(btn => {
btn.addEventListener('click', (e) => {
const docId = e.target.closest('button').dataset.id;
pendingDeleteIndex = docId;
deleteConfirmModal.style.display = 'flex';
});
});
}

// --- Подтверждение удаления ---
confirmDelete.addEventListener('click', async () => {
if (pendingDeleteIndex !== null) {
try {
await deletePost(pendingDeleteIndex);
pendingDeleteIndex = null;
deleteConfirmModal.style.display = 'none';
await loadPostsFromAppwrite();
renderAdminPostList();
showSuccess('Пост успешно удалён!');
} catch (error) {
console.error('Ошибка при удалении:', error);
}
}
});

cancelDelete.addEventListener('click', () => {
pendingDeleteIndex = null;
deleteConfirmModal.style.display = 'none';
});

adminCategory.addEventListener('change', renderAdminPostList);

newPostBtn.addEventListener('click', () => {
editingPost = null;
document.getElementById('editTitle').textContent = 'Создание поста';
document.getElementById('editErrorMessage').innerHTML = '';
postTitle.value = '';
postText.value = '';
postCode.value = '';
aiEnabled.checked = false;
aiExplanation.value = '';
imagePreview.innerHTML = '';
deletePostBtn.style.display = 'none';

const cat = adminCategory.value;
if (cat === 'scripts') {
scriptOptions.style.display = 'block';
aiInputArea.classList.add('hidden');
} else {
scriptOptions.style.display = 'none';
}
showPage('adminEditPage');
});

function editPost(docId) {
const post = allPosts.find(p => p.$id === docId);
if (!post) return;

editingPost = post;
document.getElementById('editTitle').textContent = 'Редактирование поста';
document.getElementById('editErrorMessage').innerHTML = '';
postTitle.value = post.title || '';
postText.value = post.text || '';
postCode.value = post.code || '';
aiEnabled.checked = !!post.test2;
aiExplanation.value = post.test2 || '';
imagePreview.innerHTML = post.image ? `<img src="${escapeHtml(post.image)}" style="max-width:100%; border-radius:12px; margin-top:10px;">` : '';
deletePostBtn.style.display = 'inline-flex';

const cat = post.test3;
if (cat === 'scripts') {
scriptOptions.style.display = 'block';
if (aiEnabled.checked) {
aiInputArea.classList.remove('hidden');
} else {
aiInputArea.classList.add('hidden');
}
} else {
scriptOptions.style.display = 'none';
}
showPage('adminEditPage');
}

postImage.addEventListener('change', function(e) {
const file = e.target.files[0];
if (file) {
const reader = new FileReader();
reader.onload = function(ev) {
imagePreview.innerHTML = `<img src="${ev.target.result}" style="max-width:100%; border-radius:12px; margin-top:10px;">`;
};
reader.readAsDataURL(file);
}
});

savePostBtn.addEventListener('click', async () => {
const cat = adminCategory.value;
const title = postTitle.value.trim();
const text = postText.value.trim();
const code = postCode.value.trim();
const image = imagePreview.querySelector('img') ? imagePreview.querySelector('img').src : '';

const aiEnabledValue = aiEnabled.checked;
const aiExplanationValue = aiExplanation.value.trim();

if (!title) {
showError('editErrorMessage', 'Заполните заголовок');
return;
}

if (!text) {
showError('editErrorMessage', 'Заполните основной текст поста');
return;
}

if (cat === 'scripts' && aiEnabledValue && !aiExplanationValue) {
showError('editErrorMessage', 'Заполните объяснение от ИИ или отключите эту опцию');
return;
}

const postData = {
title,
text,
code: cat === 'scripts' ? code : '',
image,
test2: cat === 'scripts' && aiEnabledValue ? aiExplanationValue : '',
test3: cat
};

try {
if (editingPost) {
await updatePost(editingPost.$id, postData);
} else {
await createPost(postData);
}
showSuccess('Пост успешно сохранён!');
await loadPostsFromAppwrite();
showPage('adminPage');
renderAdminPostList();
} catch (error) {
console.error('Ошибка при сохранении:', error);
}
});

deletePostBtn.addEventListener('click', () => {
if (editingPost) {
pendingDeleteIndex = editingPost.$id;
deleteConfirmModal.style.display = 'flex';
}
});

// --- Настройки ---
themeToggle.addEventListener('change', (e) => {
isDark = e.target.checked;
applyTheme();
});

// --- Инициализация ---
applyTheme();
showPage('homePage');

// Вспомогательная функция для экранирования HTML
function escapeHtml(unsafe) {
if (!unsafe) return unsafe;
return unsafe.replace(/[&<>"]/g, function(m) {
if (m === '&') return '&amp;';
if (m === '<') return '&lt;';
if (m === '>') return '&gt;';
if (m === '"') return '&quot;';
return m;
});
}
})();
</script>
</body>
</html>
