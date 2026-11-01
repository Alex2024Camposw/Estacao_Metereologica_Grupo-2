>[!Important]
 > `Repositório - Estação Metereológica`
>- Turma: 2° Semestre de Ciência da Computação.
>- Faculdade: Universidade Paulista.
>- Polo: UNIP Marquês.
>- Sobre: Repositório para a documentação do projeto de Estação Metereológica do 2° Semestre.
>- Membros: Alex Campos de Oliveira, Rafael Arruda, Rafael Alamino, Rafael Torso.

>[!Important]
 > `Referências`
>- `Youtube:` (URL).

<details>
<summary> HTML </summary>

<details>
<summary> Index.HTML </summary>
 
 ```csharp
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
    <link rel="stylesheet" href="css/style.css">
    <title>Dashboard-Unip</title>
</head>
<body>
    <div class="conteiner">
        <aside>
            <div class="top">
               <div class="logo">
                    <img src="img/unip-163.png" alt="">
                    <h2>UNIP <span class="badge">PRO</span></h2>
                </div>
                <div class="close" id="close-btn">
                    <span class="material-symbols-outlined">close</span>
                </div>
            </div>
            <div class="sidebar">
                <a href="index.html">
                    <span class="material-symbols-outlined">grid_view</span>
                    <h3>Dashboard</h3>
                </a>
                 <a href="ingestao.html">
                   <span class="material-symbols-outlined">tune</span>
                    <h3>Ingestão de Dados</h3>
                </a>
                 <a href="analises.html">
                    <span class="material-symbols-outlined">bar_chart</span>
                    <h3>Análises</h3>
                </a>
                 <a href="configuracoes.html">
                    <span class="material-symbols-outlined">settings</span>
                    <h3>Configurações</h3>
                </a>
                 <a href="mapa.html">
                  <span class="material-symbols-outlined">map</span>
                    <h3>Mapa</h3>
                </a>
                 <a href="logout.html">
                  <span class="material-symbols-outlined">logout</span>
                    <h3>Logout</h3>
                </a>
            </div>
        </aside>
        <!----------------------End aside------------------>
        <main>
            <h1>Dashboard</h1>
            <div class="date">
                <input id ="Date_Filter" type="date">
            </div>
            <div class="insights">
                <div class="temperature">
                    <span class="material-symbols-outlined">thermostat</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Temp.Média</h3>
                            <h1 id = "temperatura"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_temperatura"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End temperatura------------------------------>
                 <div class="humidity">
                    <span class="material-symbols-outlined">water_drops</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Umidade Média</h3>
                            <h1 id = "umidade"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_umidade"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End humidity------------------------------>
                 <div class="windspeed">
                   <span class="material-symbols-outlined">speed</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Pressão</h3>
                            <h1 id = "pressão"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_pressão"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End vento------------------------------>
                <!-----------------------End humidity------------------------------>
                 <div class="luz">
                    <span class="material-symbols-outlined">light_mode</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Luminosidade</h3>
                            <h1 id = "luminosidade"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_luminosidade"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End vento------------------------------>
                <!-----------------------End humidity------------------------------>
                 <div class="Gás">
                  <span class="material-symbols-outlined">co2</span>
                    <div class="middle">
                        <div class="left">
                            <h3>Gás</h3>
                            <h1 id = "gás"></h1>
                        </div>
                        <div class="progress">
                            <svg>
                                <circle cx='38' cy='38' r='36'></circle>
                            </svg>
                            <div class="number">
                                <p id="%_gas"></p>
                            </div>
                        </div>
                    </div>
                    <small class="text-muted">Nas últimas 24h</small>
                </div>
                <!-----------------------End gas------------------------------>
            </div>
            <!--------------------------END INSIGHTS----------------------------->
            <div class="recent-orders">
                <h2>Processamento de Dados de campo</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Estação (Nome)</th>
                            <th>Estação (ID)</th>
                            <th>Último Recebimento</th>
                        </tr>
                    </thead>
                    <tbody>
                    </tbody>
                </table>
                <a href="#">Ver tudo</a>
            </div>
        </main>
        <!---------------------END OF MAIN-------------->
        <div class="right">
            <div class="top">
                <button id="menu-btn">
                    <span class="material-symbols-outlined">menu</span>
                </button>
                <div class="theme-toggler">
                    <span class="material-symbols-outlined active">light_mode</span>
                    <span class="material-symbols-outlined">dark_mode</span>
                </div>
                <div class="profile">
                    <div class="info">
                        <p>Hey, <b>Tester</b></p>
                      
                    </div>
                    <div class="profile-photo">
                        <img src="img/profile-33.png" alt="">
                    </div>
                </div>
            </div>
            <!--end top-------->
            <div class="recent-updates">
                <h2>Recebimento Recente</h2>
                <div class="updates">
                    <div class="update">
                        <div class="profile-photo">
                            <img src="img/ESTAÇÃO.png" alt="">
                        </div>
                        <div class="message">
                            <b> <p id = "Recent_Station_Name"> </p></b>
                            <p id = "Recent_Station_Data"></p>
                            <small id = "Recent_Station_Time" class="text-muted"></small>
                        </div>
                    </div>
                    </div>
                </div>
            <!----------------END RECENT UPDATES---------------------------->
             <div class="Systems-analytics">
                <h2>Análise do Sistema</h2>
                <div class="item online">
                    <div class="icon">
                        <span class="material-symbols-outlined">language</span>
                    </div>
                    <div class="right">
                        <div class="info">
                            <b> <p id = "Analytics_Station_Name"> </p> </b>
                            <small class="text-muted" id = "Analytics_Time"> </small>
                        </div>
                        <h3 class="success" id = "Analytics_Updates_Value"> </h3>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </div>
</div>
    <script src="js/Dashboard.js"></script>
    
</body>
</html>
```
</details>

<details>
<summary> analises.html </summary>

 ```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Análises - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Análises Climáticas</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="content-card">
                <h3>Exportar Relatórios</h3>
                <p>Selecione um período para baixar os dados tratados da rede de sensoriamento.</p>
                <div class="form-group-inline">
                    <input type="date">
                    <button class="btn-primary">Gerar Relatório CSV</button>
                </div>
            </div>
        </main>
    </div>
    <script src="js/Dashboard.js"></script>
</body>
</html>
```

</details>

<details>
<summary> configuracoes.html </summary>

```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Configurações - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Configurações do Sistema</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="content-card">
                <h2>Preferências Gerais</h2>
                <form class="settings-form">
                    <div class="field">
                        <label>Unidade de Temperatura:</label>
                        <select>
                            <option>Celsius (°C)</option>
                            <option>Fahrenheit (°F)</option>
                        </select>
                    </div>
                    <div class="field checkbox-field">
                        <input type="checkbox" id="notif" checked>
                        <label for="notif">Receber notificações por E-mail</label>
                    </div>
                    <button type="button" class="btn-primary">Salvar Alterações</button>
                </form>
            </div>
        </main>
    </div>
    <script src="js/Preferencias.js"></script>
</body>
</html>
```


</details>

<details>
<summary> ingestao.html </summary>

```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ingestão De Dados - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Ingestão De Dados</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="table-card">
                <h2>Log de Transmissão de Pacotes em Tempo Real</h2>
                <div class="table-responsive">
                    <table>
                        <thead>
                            <tr>
                                <th>Origem</th>
                                <th>Protocolo</th>
                                <th>Tamanho</th>
                                <th>Status</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </main>
    </div>
    <script src="js/Dashboard.js"></script>
</body>
</html>
```


</details>


<details>
<summary> mapa.html </summary>

```csharp
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mapa Interativo - ClimaSys</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" />
    
    <!-- CSS do Leaflet -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
</head>
<body class="subpage">
    <div class="container-single">
        <main>
            <div class="page-header">
                <h1>Mapa Interativo das Estações</h1>
                <a href="index.html" class="btn-back">
                    <span class="material-symbols-outlined">arrow_back</span>
                    Voltar ao Dashboard
                </a>
            </div>

            <div class="map-card">
                <div id="map" style="width: 100%; height: 500px;"></div>
            </div>
        </main>
    </div>

    <!-- JS do Leaflet -->
    <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
    <!-- Seu JS principal -->
    <script src="js/Mapa.js"></script>
</body>
</html>
```
</details>
</details>

<details>
<summary> CSS </summary>
<details>
<summary> style.css </summary>

```csharp
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
    margin: 0;
    padding: 0;
    outline: none;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
}

:root {
    --black: #000000; 
    --red: #0468fd;
    --white: #FFFFFF;
    --gray: #867e7e;
    --color-primary: #7380ec;
    --color-danger: #ff7782;
    --color-success: #41f1b6;
    --color-warning: #ffbb55;
    --color-white: #fff;
    --color-info-dark: #7d8da1;
    --color-info-light: #dce1eb;
    --color-dark: #363949;
    --color-light: rgba(132, 139, 200, 0.18);
    --color-primary-variant: #111e88;
    --color-dark-variant: #677483;
    --color-background: #f6f6f9;

    --card-border-radius: 2rem;
    --border-radius-1: 0.4rem;
    --border-radius-2: 0.8rem;
    --border-radius-3: 1.2rem;

    --card-padding: 1.8rem;
    --padding-1: 1.2rem;

    --box-shadow: 0 2rem 3rem var(--color-light);
}

/* ---------- DARK THEME VARIABLES ---------- */
.dark-theme-variables {
    --color-background: #181a1e;
    --color-white: #202528;
    --color-dark: #edeffd;
    --color-dark-variant: #a3bdcc;
    --color-light: rgba(0, 0, 0, 0.4);
    --box-shadow: 0 2rem 3rem var(--color-light);
}

body {
    font-family: "Poppins", sans-serif;
    width: 100vw;
    min-height: 100vh;
    overflow-x: hidden;
    background-color: var(--color-background);
    user-select: none;
    color: var(--color-dark);
}


a { color: var(--color-dark); }
img { display: block; width: 100%; }

h1 { font-weight: 800; font-size: 1.8rem; }
h2 { font-size: 1.4rem; }
h3 { font-size: 0.87rem; }
h4 { font-size: 0.8rem; }
h5 { font-size: 0.77rem; }
small { font-size: 0.75rem; }

.text-muted { color: var(--color-info-dark); }
p { color: var(--color-dark-variant); }
b { color: var(--color-dark); }

.primary { color: var(--color-primary); }
.danger { color: var(--color-danger); }
.success { color: var(--color-success); }
.warning { color: var(--color-primary); }

/* ================= TELA DE LOGIN & REGISTRO ================= */
.login-background {
    background-image: url('img/fundo.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    width: 100vw;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
}

.conteiner2 {
    position: relative;
    width: 420px;
    max-width: 100%;
    height: 500px;
    background-color: transparent;
    border: 2px solid var(--red);
    border-radius: 10px;
    color: var(--red);
    padding: 30px 40px;
    box-shadow: 0 0 10px rgba(0, 0, 0, .2);
    backdrop-filter: blur(5px);
    overflow: hidden;
    transition: height .4s ease, border-color 0.5s ease;
}

.conteiner2.active {
    height: 580px;
}

.conteiner2 h1 {
    font-size: 36px;
    text-align: center;
}

.input-box {
    position: relative;
    width: 100%;
    height: 50px;
    margin: 20px 0;
}

.input-box input {
    width: 100%;
    height: 100%;
    background-color: transparent;
    border: 1px solid var(--black); 
    border-radius: 40px;
    outline: none;
    font-size: 16px;
    color: #FFFFFF;
    padding: 0 45px 0 20px; 
}

.input-box input::placeholder {
    color: var(--gray);
}

.input-box i {
    position: absolute;
    right: 20px;
    font-size: 20px;
    top: 50%;
    transform: translateY(-50%);
}

.remember-forgot {
    display: flex;
    justify-content: space-between;
    font-size: 14px;
    margin: -5px 0 15px;
}

.remember-forgot label input {
    accent-color: var(--white);
    margin-right: 5px;
}

.remember-forgot a {
    color: var(--gray);
}

.remember-forgot a:hover {
    text-decoration: underline;
}

.Loginbutton {
    width: 100%;
    height: 50px;
    background-color: var(--red);
    border: none;
    border-radius: 40px;
    cursor: pointer;
    font-size: 16px;
    color: var(--white);
    font-weight: 600;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
    margin-top: 10px;
    transition: 0.3s;
}

.Loginbutton:hover {
    background-color: transparent;
    border: 2px solid rgba(255, 255, 255, .2);
    color: var(--black);
}

.register-link {
    font-size: 14px;
    text-align: center;
    margin: 20px 0 15px;
}

.register-link a {
    color: var(--gray);
    font-weight: 600;
}

.register-link a:hover {
    text-decoration: underline;
}

.conteiner2:hover {
    border-color: var(--white);
    animation: border-glow 1s infinite alternate;
}

@keyframes border-glow {
    from {
        border-color: var(--red);
        box-shadow: 0 0 20px rgba(0,0,0,0.5);
    }
    to {
        border-color: var(--red);
        box-shadow: 0 0 20px rgba(255, 255, 255, .1);
    }
}

.form-box {
    width: 100%;
    transition: transform .5s ease;
}

.conteiner2 .form-box.login {
    transform: translateX(0);
}

.conteiner2.active .form-box.login {
    transform: translateX(-500px);
}

.conteiner2 .form-box.register {
    position: absolute;
    top: 30px;
    left: 40px;
    right: 40px;
    width: calc(100% - 80px);
    transform: translateX(500px);
}

.conteiner2.active .form-box.register {
    transform: translateX(0);
}

.form-box.register .icon-close {
    position: absolute;
    top: -10px;
    left: -15px;
    width: 35px;
    height: 35px;
    background: var(--red);
    font-size: 1.6em;
    color: var(--white);
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    cursor: pointer;
    z-index: 10;
    transition: background 0.3s ease, transform 0.2s ease;
}

.form-box.register .icon-close:hover {
    background: var(--black);
    transform: scale(1.1);
}

/* ================= DASHBOARD LAYOUT ================= */
.conteiner {
    display: grid;
    width: 96%;
    margin: 0 auto;
    gap: 1.8rem;
    grid-template-columns: 14rem auto 23rem;
}

/* ---------- SIDEBAR ---------- */
aside {
    height: 100vh;
}

aside .top {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 1.4rem;
}

aside .logo {
    display: flex;
    gap: 0.8rem;
}

aside .logo img {
    width: 6rem;
    height: 6rem;
}

aside .close {
    display: none;
}

aside .logo h2 {
    display: flex;
    align-items: center;
    gap: 0.5rem;
}

aside .logo .badge {
    background: var(--color-primary, #7380ec);
    color: #fff;
    font-size: 0.65rem;
    padding: 0.2rem 0.5rem;
    border-radius: 0.4rem;
    font-weight: 600;
    text-transform: uppercase;
}

aside .sidebar {
    display: flex;
    flex-direction: column;
    height: calc(100vh - 6rem);
    position: relative;
    top: 3rem;
}

aside h3 {
    font-weight: 500;
}

aside .sidebar a {
    display: flex;
    color: var(--color-info-dark);
    margin-left: 2rem;
    gap: 1.2rem;
    align-items: center;
    position: relative;
    height: 4rem;
    transition: all 300ms ease;
}

aside .sidebar a span {
    font-size: 1.8rem;
    transition: all 300ms ease;
}

aside .sidebar a h3 {
    font-size: 1rem;
    font-weight: 500;
}

aside .sidebar a:last-child {
    position: absolute;
    bottom: 1rem;
    width: 100%;
}

aside .sidebar a.active {
    background: var(--color-light);
    color: var(--color-primary);
    margin-left: 0;
}

aside .sidebar a.active::before {
    content: "";
    width: 8px;
    height: 100%;
    background: var(--color-primary, #7380ec);
    position: absolute;
    left: 0;
    top: 0;
    border-radius: 0 4px 4px 0;
}

aside .sidebar a.active span {
    color: var(--color-primary);
    margin-left: calc(1rem - 3px);
}

aside .sidebar a:hover {
    color: var(--color-primary);
}

aside .sidebar a:hover span {
    margin-left: 1rem;
}

/* ---------- MAIN CONTENT & BOTÃO VOLTAR ---------- */
main {
    margin-top: 1.4rem;
}

.page-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.8rem;
    flex-wrap: wrap;
    gap: 1rem;
}

.btn-back {
    display: inline-flex;
    align-items: center;
    gap: 0.5rem;
    background: var(--color-primary);
    color: var(--color-white);
    padding: 0.6rem 1.2rem;
    border-radius: var(--border-radius-1);
    font-weight: 500;
    transition: all 300ms ease;
}

.btn-back:hover {
    opacity: 0.85;
    transform: translateX(-3px);
}

main .date {
    display: inline-block;
    background: var(--color-light);
    border-radius: var(--border-radius-1);
    margin-top: 1rem;
    padding: 0.3rem 1rem;
    box-shadow: 0 0.5rem 1rem var(--color-light);
}

main .date input[type='date'] {
    background: transparent;
    color: var(--color-dark);
    border: none;
    outline: none;
    font-family: inherit;
    font-size: 0.9rem;
    cursor: pointer;
}

.date input[type="date"]::-webkit-calendar-picker-indicator {
    cursor: pointer;
    filter: invert(0.4);
}

main .insights {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.6rem;
}

main .insights > div {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    margin-top: 1rem;
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

main .insights > div:hover {
    box-shadow: none;
}

main .insights > div span {
    background: red;
    padding: 0.5rem;
    border-radius: 50%;
    color: var(--color-white);
    font-size: 2rem;
}

main .insights > div.humidity span {
    background: var(--red);
}

main .insights > div.windspeed span {
    background: var(--color-warning);
}

main .insights > div.luz span {
    background: #eeff55; /* Fundo Amarelo do Ícone */
}

main .insights > div.Gás span {
    background: #867e7e; /* Fundo Cinza do Ícone */
}

main .insights > div .middle {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

main .insights > div .left {
    margin-right: 0.1rem;
}

main .insights h3 {
    margin: 1rem 0 0.6rem;
    font-size: 1rem;
}

main .insights .progress {
    position: relative;
    width: 92px;
    height: 92px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}

main .insights svg {
    width: 92px;
    height: 92px;
    transform: rotate(-90deg);
}

main .insights svg circle {
    fill: none;
    stroke-width: 10;
    stroke-linecap: round;
    transform: translate(8px, 8px);
    
    /* Circunferência total do raio 36 */
    stroke-dasharray: 226; 
    
    /* Valor inicial (0% visível) */
    stroke-dashoffset: 226; 
    
    /* Animação suave ao alterar o valor */
    transition: stroke-dashoffset 1s ease-in-out; 
}

main .insights .temperature svg circle {
    stroke: #ff5252;
    filter: drop-shadow(0px 3px 6px rgba(255, 82, 82, 0.4));
    stroke-dashoffset: -30;
    stroke-dasharray: 200;
}

main .insights .humidity svg circle {
    stroke: #0468fd;
    filter: drop-shadow(0px 3px 6px rgba(4, 104, 253, 0.45));
    stroke-dashoffset: 20;
    stroke-dasharray: 80;
}

main .insights .windspeed svg circle {
   stroke: #ff7700; /* Círculo de Progresso Laranja */
    filter: drop-shadow(0px 3px 6px rgba(255, 119, 0, 0.45));
    stroke-dashoffset: 45;
    stroke-dasharray: 90;
}

main .insights .luz svg circle {
    stroke: #fffc3a; /* Círculo de Progresso Amarelo */
    filter: drop-shadow(0px 3px 6px rgba(255, 187, 85, 0.45));
    stroke-dashoffset: 45;
    stroke-dasharray: 90;
}

main .insights .Gás svg circle {
    stroke: #867e7e; /* Círculo de Progresso Cinza */
    filter: drop-shadow(0px 3px 6px rgba(134, 126, 126, 0.45));
    stroke-dashoffset: 45;
    stroke-dasharray: 90;
}

main .insights .progress .number {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0;
    padding: 0;
}

main .insights .progress .number p {
    font-weight: 600;
    font-size: 0.85rem;
    line-height: 1;
}

main .insights small {
    margin-top: 1.3rem;
    display: block;
}

/* ---------- TABELAS / RECENT ORDERS ---------- */
main .recent-orders {
    margin-top: 2rem;
    overflow-x: auto;
}

main .recent-orders h2 {
    margin-bottom: 0.8rem;
}

main .recent-orders table {
    background: var(--color-white);
    width: 100%;
    border-radius: var(--card-border-radius);
    padding: var(--card-padding);
    text-align: center;
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

main .recent-orders table:hover {
    box-shadow: none;
}

main table tbody td {
    height: 2.8rem;
    border-bottom: 1px solid var(--color-light);
    color: var(--color-dark-variant);
}

main table tbody tr:last-child td {
    border: none;
}

main .recent-orders a {
    text-align: center;
    display: block;
    margin: 1rem auto;
    color: var(--color-primary);
}

/* ---------- DIREITA / RIGHT PANEL ---------- */
.right {
    margin-top: 1.4rem;
}

.right .top {
    display: flex;
    justify-content: end;
    gap: 2rem;
}

.right .top button {
    display: none;
}

.right .theme-toggler {
    background: var(--color-light);
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 1.6rem;
    width: 4.2rem;
    cursor: pointer;
    border-radius: var(--border-radius-1);
}

.right .theme-toggler span {
    font-size: 1.2rem;
    width: 50%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.right .profile {
    display: flex;
    gap: 1rem;
    align-items: center;
    text-align: right;
}

.right .profile .info p {
    margin: 0;
    font-size: 0.9rem;
}

.right .profile .info small {
    display: block;
    margin-top: -2px;
}

.right .profile-photo {
    width: 2.8rem;
    height: 2.8rem;
    border-radius: 50%;
    overflow: hidden;
}

.right .profile-photo img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transform: scale(6.2);
}

.right .theme-toggler span.active {
    background: var(--color-primary);
    color: white;
    border-radius: var(--border-radius-1);
}

.right .recent-updates {
    margin-top: 1rem;
}

.right .recent-updates h2 {
    margin-bottom: 0.8rem;
}

.right .recent-updates .updates {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

.right .recent-updates .updates:hover {
    box-shadow: none;
}

.right .recent-updates .updates .update {
    display: grid;
    grid-template-columns: 2.6rem auto;
    gap: 1rem;
    margin-top: 1rem;
}

.right .Systems-analytics {
    margin-top: 2rem;
}

.right .Systems-analytics h2 {
    margin-bottom: 0.8rem;
}

.right .Systems-analytics .item {
    background: var(--color-white);
    display: flex;
    align-items: center;
    gap: 1rem;
    margin-bottom: 0.7rem;
    padding: 1.4rem var(--card-padding);
    border-radius: var(--border-radius-3);
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

.right .Systems-analytics .item:hover {
    box-shadow: none;
}

.right .Systems-analytics .item .right {
    display: flex;
    justify-content: space-between;
    align-items: start;
    margin: 0;
    width: 100%;
}

.right .Systems-analytics .item .icon {
    padding: 0.6rem;
    color: var(--color-white);
    border-radius: 50%;
    background: var(--color-primary);
    display: flex;
}

.right .Systems-analytics .item.offline .icon {
    background: var(--color-danger);
}

.right .Systems-analytics .item.customers .icon {
    background: var(--color-success);
}

/* ================= ESTRUTURAS DAS PÁGINAS SECUNDÁRIAS ================= */

/* Layout sem Sidebar */
.container-single {
    width: 92%;
    max-width: 1200px;
    margin: 2rem auto;
    display: block;
}

/* Cards de Conteúdo Gerais */
.content-card, 
.table-card, 
.map-card,
.form-container, 
.form-card {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    margin-top: 1rem;
    width: 100%;
}

/* Mapa Interativo (Leaflet/Google Maps) */
#map {
    width: 100%;
    height: 520px;
    border-radius: var(--border-radius-2);
    z-index: 1;
}

/* Tabelas Responsivas para Subpáginas */
.table-responsive,
.table-container {
    width: 100%;
    overflow-x: auto;
    margin-top: 1rem;
}

.table-responsive table,
.table-container table {
    width: 100%;
    border-collapse: collapse;
    text-align: left;
}

.table-responsive th, .table-responsive td,
.table-container th, .table-container td {
    padding: 1rem;
    border-bottom: 1px solid var(--color-light);
}

.table-responsive th, .table-container th {
    color: var(--color-info-dark);
    font-weight: 600;
}

.badge-status {
    padding: 0.3rem 0.8rem;
    border-radius: var(--border-radius-1);
    font-size: 0.8rem;
    font-weight: 600;
}

.badge-status.success { background: rgba(65, 241, 182, 0.2); color: #0d9467; }
.badge-status.danger { background: rgba(255, 119, 130, 0.2); color: #d32f2f; }

/* Formulários das Páginas Secundárias */
.form-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.2rem;
    margin-bottom: 1.5rem;
}

.form-group {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
}

.form-group input, 
.form-group select, 
.form-group textarea,
.settings-form select, 
.settings-form input[type="date"] {
    width: 100%;
    padding: 0.8rem 1rem;
    border-radius: var(--border-radius-1);
    border: 1px solid var(--color-info-light);
    background: var(--color-background);
    color: var(--color-dark);
    font-family: inherit;
    font-size: 0.9rem;
}

.form-actions {
    display: flex;
    gap: 1rem;
    justify-content: flex-end;
    flex-wrap: wrap;
}

.btn-primary {
    padding: 0.8rem 1.5rem;
    background: var(--color-primary);
    color: var(--color-white);
    border: none;
    border-radius: var(--border-radius-1);
    cursor: pointer;
    font-weight: 600;
    transition: opacity 300ms ease;
}

.btn-primary:hover {
    opacity: 0.9;
}

/* Grids de Cards / Analytics */
.cards-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 1.6rem;
    margin-top: 1rem;
}

.card-item {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    transition: all 300ms ease;
}

.card-item:hover {
    box-shadow: none;
}

.chart-container {
    background: var(--color-white);
    padding: var(--card-padding);
    border-radius: var(--card-border-radius);
    box-shadow: var(--box-shadow);
    margin-top: 1rem;
    position: relative;
    width: 100%;
    min-height: 320px;
}

/* ================= MEDIA QUERIES (RESPONSIVIDADE COMPLETA) ================= */

/* Login - Celulares */
@media (max-width: 480px) {
    .conteiner2 {
        padding: 25px 20px;
    }

    .conteiner2 .form-box.register {
        left: 20px;
        right: 20px;
        width: calc(100% - 40px);
    }

    .conteiner2 h1 {
        font-size: 28px;
    }

    .remember-forgot {
        font-size: 12px;
        flex-direction: column;
        gap: 8px;
    }

    .form-box.register .icon-close {
        left: -5px;
        top: -15px;
    }

    .form-actions {
        flex-direction: column;
    }

    .form-actions button, 
    .form-actions a {
        width: 100%;
        text-align: center;
    }
}

/* Dashboard & Layout - Notebooks / Tablets Grandes */
@media screen and (max-width: 1200px) {
    .conteiner {
        width: 94%;
        grid-template-columns: 7rem auto 23rem;
    }

    aside .logo h2,
    aside .sidebar h3 {
        display: none;
    }

    aside .sidebar a {
        width: 5.6rem;
    }

    aside .sidebar a:last-child {
        position: relative;
        margin-top: 1.8rem;
    }

    main .insights {
        grid-template-columns: 1fr;
        gap: 0;
    }

    main .recent-orders {
        width: 94%;
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        margin: 2rem 0 0 8.8rem;
    }

    main .recent-orders table {
        width: 83vw;
    }

    main table thead tr th:first-child,
    main table tbody tr td:first-child,
    main table thead tr th:last-child,
    main table tbody tr td:last-child {
        display: none;
    }
}

/* Dashboard & Páginas Secundárias - Celulares e Tablets */
@media screen and (max-width: 768px) {
    .conteiner {
        width: 100%;
        grid-template-columns: 1fr;
        padding-top: 4rem;
    }

    .container-single {
        width: 95%;
        padding: 0 0.5rem;
        margin-top: 1rem;
    }

    aside {
        position: fixed;
        left: -100%;
        background: var(--color-white);
        width: 18rem;
        z-index: 10;
        box-shadow: 1rem 3rem 4rem var(--color-light);
        height: 100vh;
        padding-right: var(--card-padding);
        display: none;
        animation: showMenu 400ms ease forwards;
    }
    
    aside .sidebar a:last-child {
        position: relative; /* Mudado de absolute para relative no mobile */
        bottom: 0;
        margin-top: 2rem;
        margin-bottom: 2rem;
    }


    @keyframes showMenu {
        to {
            left: 0;
        }
    }

    aside .logo {
        margin-left: 1rem;
    }
    
    aside .logo h2,
    aside .sidebar h3 {
        display: inline;
    }

    aside .sidebar a {
        width: 100%;
        height: 3.4rem;
    }

    aside .sidebar a:last-child {
        position: absolute;
        bottom: 5rem;
    }

    aside .close {
        display: inline-block;
        cursor: pointer;
    }

    main {
        margin-top: 1rem;
        padding: 0 1rem;
    }

    .page-header {
        flex-direction: column;
        align-items: flex-start;
    }

    .btn-back {
        width: 100%;
        justify-content: center;
    }

    #map {
        height: 380px;
    }

    main .recent-orders {
        position: relative;
        margin: 2rem 0 0 0;
        width: 100%;
        overflow-x: auto;
    }

    main .recent-orders table {
        width: 100%;
        margin: 0;
    }

    main table thead tr th:first-child,
    main table tbody tr td:first-child,
    main table thead tr th:last-child,
    main table tbody tr td:last-child {
        display: none;
    }

    .right {
        width: 100%;
        margin: 0 auto 4rem;
        padding: 0 1rem;
    }

    .right .top {
        position: fixed;
        top: 0;
        left: 0;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 1.5rem;
        height: 4.6rem;
        background: var(--color-white);
        width: 100%;
        margin: 0;
        z-index: 5;
        box-shadow: 0 0.5rem 1rem var(--color-light);
    }

    .right .top button {
        display: flex;
        align-items: center;
        justify-content: center;
        background: transparent;
        border: none;
        cursor: pointer;
        color: var(--color-dark);
        position: static;
    }

    .right .top button span {
        font-size: 2rem;
    }

    .right .top .theme-toggler {
        width: 4.4rem;
        position: static;
    }

    .right .profile .info {
        display: none;
    }

    .form-grid,
    .cards-grid {
        grid-template-columns: 1fr;
    }
}
/* ==========================================================================
   ESTILOS DO MAPA INTERATIVO (LEAFLET)
   ========================================================================== */
#map {
    width: 100%;
    height: 500px;
    border-radius: 1rem;
    z-index: 1;
}

.map-card {
    width: 100%;
    min-height: 500px;
}
```

</details>


</details>

<details>
<summary> SQL </summary>

<details>
<summary> Estacao_Metereologica.sql </summary>

```csharp
create database Estacao_Meteorologica;
use Estacao_Meteorologica;

SET SQL_SAFE_UPDATES = 0;

create table tbEstacao(
Id_Estacao int (10) primary key,
Nome_Estacao char (100) not null,
latitude float (4,2),
longitude float (4,2)	
);

create table tbLeitura(
 Id_Leitura BigInt primary key auto_increment,
 Id_Estacao int (10) not null,
 temperatura float (4,2),
 qualidade_ar int,
 luminosidade int,
 umidade float (4,2),
 pressao float (4,2),
 data_hora timestamp,

 foreign key (Id_Estacao) references tbEstacao(Id_Estacao)
);

select * from tbLeitura;

select * from tbEstacao;

SELECT Id_Estacao FROM tbEstacao ORDER BY Id_Estacao;

select data_hora from tbLeitura;

select * from tbLeitura;

select * from tbEstacao;

use Estacao_Meteorologica;

select * from tbLeitura;

select * from tbEstacao;

SELECT Id_Estacao FROM tbEstacao ORDER BY Id_Estacao;

select data_hora from tbLeitura;

select * from tbLeitura;

select * from tbEstacao;
SELECT *
FROM tbLeitura
WHERE DATE(data_hora) = '2026-09-30';
```

</details>

</details>

<details>
<summary> Back-End </summary>
 <details>
<summary> Main_Back.py </summary>
  
```csharp
from js.Back_End.Dados import Dado
from js.Back_End.Filtragem import Filtrar_Dados
from js.Back_End.Data import Verificar_Data, Formatar_para_Padrao
from js.Back_End.Banco import (
    Inserir_Dados_no_Banco,
    Puxar_Data,
    Puxar_Id,
    Puxar_Historico,
    Puxar_Nome_Estacao
)
from js.Back_End.HTTP import API

from flask import Flask, request, jsonify
from flask_cors import CORS
from dotenv import load_dotenv

import os
import time
import threading
import math

def Limpar_Valores_JSON(dados):
    if isinstance(dados, dict):
        return {
            chave: Limpar_Valores_JSON(valor)
            for chave, valor in dados.items()
        }

    if isinstance(dados, list):
        return [Limpar_Valores_JSON(valor) for valor in dados]

    if isinstance(dados, float) and not math.isfinite(dados):
        return None

    return dados

load_dotenv()
app = Flask(__name__)

Origens_Permitidas = [
    "http://127.0.0.1:5500",
    "http://localhost:5500",
    "https://projetos-estacao-meteorol-gica-grupo-3de5.vercel.app"
]

CORS(app, origins=Origens_Permitidas)
PORT = int(os.getenv("PORT", 3000))


dados_API, Status_Code = API.Buscar_Dados_HTTP(True)

Lista_de_Dados = []

Temperatura = None
Umidade = None
Luminosidade = None
Gas = None
Pressao = None

Qtd_Campos_Atualizados = 0

Historico_de_Dados = Puxar_Historico()
Valores_Leitura = []
Valores_Estacao = []

API_ID_Anterior = dados_API["channel"]["last_entry_id"]
API_Novo_ID = dados_API["channel"]["last_entry_id"]

Dados_Atualizados = False

Id_Estacao = Puxar_Id("tbEstacao")

Nome_Estacao = dados_API["channel"]["name"]
latitude = dados_API["channel"]["latitude"]
longitude = dados_API["channel"]["longitude"]

Data_Hora_Atual = None
Data_Hora_Anterior = Puxar_Data()

if Id_Estacao is None:
    Id_Estacao = dados_API["channel"]["id"]

    Valores_Estacao = [
        Id_Estacao,
        Nome_Estacao,
        latitude,
        longitude
    ]

    Inserir_Dados_no_Banco(
        Valores_Estacao,
        "tbEstacao"
    )

else:
    print("Estacao ja existe.")

if Status_Code == 200:
    Lista_de_Dados.extend([
        Dado("field1", dados_API["feeds"]),
        Dado("field2", dados_API["feeds"]),
        Dado("field3", dados_API["feeds"]),
        Dado("field6", dados_API["feeds"]),
        Dado("field7", dados_API["feeds"])
    ])
    Temperatura = Lista_de_Dados[0]
    Umidade = Lista_de_Dados[1]
    Luminosidade = Lista_de_Dados[2]
    Gas = Lista_de_Dados[3]
    Pressao = Lista_de_Dados[4]


def Atualizar_Objetos():
    global Qtd_Campos_Atualizados

    Temperatura.Atualizar_Dados(dados_API["feeds"])
    Umidade.Atualizar_Dados(dados_API["feeds"])
    Luminosidade.Atualizar_Dados(dados_API["feeds"])
    Gas.Atualizar_Dados(dados_API["feeds"])
    Pressao.Atualizar_Dados(dados_API["feeds"])

    Qtd_Campos_Atualizados = Dado.Qtd_Atualizado

    Dado.Zerar_Contabilizador()

def Montar_Valores_Banco():
    for Element in Lista_de_Dados:
        Element.Campo_Valor = [
            None if math.isnan(Valor) else Valor
            for Valor in Element.Campo_Valor
        ]

    return [
        Id_Estacao,
        Temperatura.Campo_Valor[-1],
        Gas.Campo_Valor[-1],
        Luminosidade.Campo_Valor[-1],
        Umidade.Campo_Valor[-1],
        Pressao.Campo_Valor[-1],
        Data_Hora_Atual
    ]

def Atualizar_Banco():
    global Valores_Leitura
    global Historico_de_Dados
    global Nome_Estacao

    Valores_Leitura = Montar_Valores_Banco()

    Inserir_Dados_no_Banco(
        Valores_Leitura,
        "tbLeitura"
    )

    Historico_de_Dados = Puxar_Historico()
    Nome_Estacao = Puxar_Nome_Estacao()

def Main():
    global dados_API
    global Status_Code
    global API_Novo_ID
    global API_ID_Anterior
    global Data_Hora_Atual
    global Data_Hora_Anterior
    global Dados_Atualizados

    while True:
        time.sleep(10)

        Dado.Zerar_Contabilizador()

        dados_API, Status_Code = API.Buscar_Dados_HTTP(True)

        if Status_Code != 200:
            print("Erro ao consultar a API:", Status_Code)
            continue

        API_Novo_ID = dados_API["channel"]["last_entry_id"]

        if API_Novo_ID == API_ID_Anterior:
            print("Nenhuma atualizacao.")
            continue

        Data_Hora_Atual = Formatar_para_Padrao(
            dados_API["feeds"][-1]["created_at"]
        )

        print("Data-Hora:", Data_Hora_Atual)

        if Verificar_Data(
            Data_Hora_Anterior,
            Data_Hora_Atual
        ):
            print("Dado repetido")
            print("Historico Obtido:", Historico_de_Dados)
            API_ID_Anterior = API_Novo_ID
            continue

        else:
            print("Novo dado encontrado")

            API_ID_Anterior = API_Novo_ID
            Data_Hora_Anterior = Data_Hora_Atual

            Dados_Atualizados = True

            Atualizar_Objetos()
            Atualizar_Banco()

            print("Estado da Atualizacao:", Dados_Atualizados)
            print("ID Novo:", API_Novo_ID)
            print("ID Anterior:", API_ID_Anterior)

@app.route("/dados", methods=["GET"])
def Obter_Dados():
    global Dados_Atualizados

    if request.args.get("data"):
        return Filtrar_Dados(request, jsonify)

    resposta = {
        "Nome_Estacao": Nome_Estacao,
        "temperatura": Temperatura.Campo_Valor[-1],
        "umidade": Umidade.Campo_Valor[-1],
        "luminosidade": Luminosidade.Campo_Valor[-1],
        "gás": Gas.Campo_Valor[-1],
        "pressão": Pressao.Campo_Valor[-1],
        "Qtd_Atualizados": Qtd_Campos_Atualizados,
        "Historico_de_Dados": Historico_de_Dados,
        "Data_Hora": Data_Hora_Atual,
        "Atualizacao": Dados_Atualizados,
        "Codigo_HTTP": Status_Code,
        "latitude": latitude,
        "longitude": longitude
    }

    Dados_Atualizados = False
    return jsonify(Limpar_Valores_JSON(resposta))

if __name__ == "__main__":
    threading.Thread(
        target=Main,
        daemon=True
    ).start()

    app.run(
        host="0.0.0.0",
        port=PORT,
        debug=False,
        use_reloader=False
    )
```

</details>
<details>
<summary> Banco.py </summary>

```csharp
import os
import mysql.connector
from dotenv import load_dotenv
from datetime import datetime
from js.Back_End.Data import Formatar_para_MYSQL

# Carrega as variáveis de ambiente
load_dotenv()

# Cria a conexão com o banco de dados
conexao = mysql.connector.connect(
    host=os.getenv("DB_host"),
    port=os.getenv("DB_port"),
    user=os.getenv("DB_user"),
    password=os.getenv("DB_password"),
    database=os.getenv("DB_database")
)

# As funções abaixo executam SELECTs e INSERTs no banco de dados.


# Busca o nome da estação
def Puxar_Nome_Estacao():
    cursor = conexao.cursor(dictionary=True)

    try:
        Select_Nome_Estacao = """
            SELECT Nome_Estacao
            FROM tbEstacao;
        """

        cursor.execute(Select_Nome_Estacao)
        resultado = cursor.fetchall()

        print("Estação:", resultado)

        if resultado:
            return resultado[0]["Nome_Estacao"]

        return None

    except mysql.connector.Error as erro:
        print("Erro ao buscar estação:", erro)
        raise

    finally:
        cursor.close()


# Busca todo o histórico de leituras
def Puxar_Historico():
    cursor = conexao.cursor(dictionary=True)

    try:
        Historico_Select = """
            SELECT Id_Estacao, temperatura, qualidade_ar,
                   luminosidade, umidade, pressao, data_hora
            FROM tbLeitura;
        """

        cursor.execute(Historico_Select)
        resultado = cursor.fetchall()

        print("Histórico Puxado no Banco:", resultado)

        return resultado

    except mysql.connector.Error as erro:
        print("Erro ao puxar histórico:", erro)
        raise

    finally:
        cursor.close()


# Busca as leituras de uma data específica
def Pegar_Dados_Filtrados(Data_do_Filtro):
    cursor = conexao.cursor(dictionary=True)

    try:
        Data_do_Filtro = Formatar_para_MYSQL(Data_do_Filtro)

        if Data_do_Filtro is None:
            return []

        # Extrai somente a data: YYYY-MM-DD
        Data_do_Filtro = Data_do_Filtro[:10]

        Select_Dados = """
            SELECT *
            FROM tbLeitura
            WHERE DATE(data_hora) = %s;
        """

        cursor.execute(Select_Dados, (Data_do_Filtro,))
        resultado = cursor.fetchall()

        return resultado

    except mysql.connector.Error as erro:
        print("MYSQL ERRO:", erro)
        raise

    finally:
        cursor.close()


# Busca a data da leitura mais recente
def Puxar_Data():
    cursor = conexao.cursor(dictionary=True)

    try:
        Data_Select = """
            SELECT data_hora
            FROM tbLeitura
            ORDER BY data_hora DESC
            LIMIT 1;
        """

        cursor.execute(Data_Select)
        resultado = cursor.fetchone()

        # Não existe nenhuma leitura no banco
        if resultado is None:
            print("Nenhuma leitura encontrada.")
            return None

        # Existe uma leitura
        Data = resultado["data_hora"]

        if isinstance(Data, datetime):
            Data_Formatada = Data.strftime("%Y-%m-%d %H:%M:%S")
        else:
            Data_Formatada = str(Data)

        print("Resultado Retornado:", Data_Formatada)

        return Data_Formatada

    except mysql.connector.Error as erro:
        print("Erro ao buscar data:", erro)
        raise

    finally:
        cursor.close()


# Busca o primeiro ID da tabela informada
def Puxar_Id(Tabela):
    cursor = conexao.cursor(dictionary=True)

    try:
        if Tabela == "tbLeitura":
            Coluna_Id = "Id_Leitura"
        elif Tabela == "tbEstacao":
            Coluna_Id = "Id_Estacao"
        else:
            raise ValueError("Tabela inválida.")

        Id_Tabela = f"""
            SELECT {Coluna_Id}
            FROM {Tabela}
            ORDER BY {Coluna_Id}
            LIMIT 1;
        """

        cursor.execute(Id_Tabela)
        resultado = cursor.fetchone()

        if resultado is None:
            return None

        return resultado[Coluna_Id]

    except mysql.connector.Error as erro:
        print("Erro ao buscar ID:", erro)
        raise

    finally:
        cursor.close()


# Insere dados no banco de dados
def Inserir_Dados_no_Banco(Dados_Leitura, Tabela):
    cursor = conexao.cursor()

    try:
        if Tabela == "tbEstacao":
            Leitura = """
                INSERT INTO tbEstacao
                (Id_Estacao, Nome_Estacao, Latitude, Longitude)
                VALUES (%s, %s, %s, %s);
            """

        elif Tabela == "tbLeitura":
            Leitura = """
                INSERT INTO tbLeitura
                (Id_Estacao, temperatura, qualidade_ar,
                 luminosidade, umidade, pressao, data_hora)
                VALUES (%s, %s, %s, %s, %s, %s, %s);
            """

        else:
            raise ValueError("Tabela inválida.")

        cursor.execute(Leitura, Dados_Leitura)
        conexao.commit()

        print("Dados inseridos no Banco:", cursor.lastrowid)

        return cursor.lastrowid

    except Exception as erro:
        conexao.rollback()
        print("Erro ao inserir:", erro)
        raise

    finally:
        cursor.close()


# Verifica se a conexão está ativa
if conexao.is_connected():
    print("Conectado ao MySQL!")


# Encerra a conexão quando necessário
def Fechar_Conexao():
    if conexao.is_connected():
        conexao.close()
        print("Conexão com MySQL encerrada.")
```

</details>
<details>
<summary> Dados.py </summary>

```csharp
class Dado:
    Qtd_Atualizado = 0
    def __init__(self, Campo_Tipo, Ref_Dados):
        self.Campo_Tipo = Campo_Tipo
        self.Campo_Data = []
        self.Campo_Valor = []
        self.Adicionar_Dados(Ref_Dados)

    def Adicionar_Dados(self, Ref_Dado):
        for Dados in Ref_Dado:
            try:
                Valor_Float = float(Dados[self.Campo_Tipo])
            except (ValueError, TypeError):
                Valor_Float = float("nan")

            self.Campo_Valor.append(Valor_Float)
            self.Campo_Data.append(Dados["created_at"])

    def Atualizar_Dados(self, Ref_Dados):
        self.Campo_Valor = []
        self.Campo_Data = []

        Dado.Zerar_Contabilizador()

        for Dados in Ref_Dados:
            try:
                Valor_Float = float(Dados[self.Campo_Tipo])
            except (ValueError, TypeError):
                Valor_Float = float("nan")

            self.Campo_Valor.append(Valor_Float)
            self.Campo_Data.append(Dados["created_at"])

            Dado.Contabilizar_Campos_Registrados()

    @staticmethod
    def Contabilizar_Campos_Registrados():
        Dado.Qtd_Atualizado += 1
        return Dado.Qtd_Atualizado

    @staticmethod
    def Zerar_Contabilizador():
        Dado.Qtd_Atualizado = 0
        return Dado.Qtd_Atualizado
```

</details>
<details>
<summary> Data.py </summary>

```csharp
def Verificar_Data(Data_Anterior, Data_Atual):
    print(f"{Data_Atual} : {Data_Anterior}")

    if Data_Atual == Data_Anterior:
        print("Datas Iguais. Interrompido")
        return True
    else:
        print("Datas diferentes. Dar seguimento")
        return False


def Formatar_para_MYSQL(Data_Normal):
    if not Data_Normal:
        return None

    return f"{Data_Normal} 00:00:00"


def Formatar_para_Padrao(data):
    if not data:
        return None

    return data.replace("T", " ").replace("Z", "")
```

</details>
<details>
<summary> Filtragem.py </summary>

```csharp
from flask import request, jsonify
from js.Back_End.Banco import Pegar_Dados_Filtrados

def Filtrar_Dados():
    Data_para_Filtrar = request.args.get("data")

    try:
        Dados_Filtrados = Pegar_Dados_Filtrados(Data_para_Filtrar)

        print("DADOS:", Dados_Filtrados)

        return jsonify(Dados_Filtrados)

    except Exception as erro:
        print("Erro ao filtrar:", erro)

        return jsonify({
            "erro": "Erro ao buscar dados filtrados"
        }), 500

```

</details>
<details>
<summary> HTTP.py </summary>

```csharp
import os
import requests
from dotenv import load_dotenv
load_dotenv()

class HTTP:
    def __init__(self, URL):
        self.URL = URL
        
    def Buscar_Dados_HTTP(self, Pegar_HTTP=False):
        resposta = requests.get(self.URL)
        dados = resposta.json()

        if Pegar_HTTP is True:
            HTTP_Status = resposta.status_code
            return dados, HTTP_Status

        return None

    def Buscar_Dados(self):
        resposta = requests.get(self.URL)
        dados = resposta.json()
        return dados
    
API = HTTP(os.getenv("API_URL"))
```

</details>
</details>

<details>
<summary> Front-End </summary>
<details>
<summary> Dashboard.js </summary>

```csharp
let dados;
let Registro_do_Historico = [];
let Pausar_Atualização = false;
let Contador_Registros;
let Ultimo_Dado;

const RENDER_URL = "https://projetos-estacao-meteorol-gica.onrender.com/dados";
const Filtro_de_Data = document.getElementById("Date_Filter");

if (Filtro_de_Data) {
    Filtro_de_Data.addEventListener("change", Filtrar_por_Data);
} else {
    console.log("Botão de filtrar não encontrado");
}

async function Buscar_Dados() {
    // Verifica se o Flask respondeu corretamente.
    const resposta = await fetch(RENDER_URL);

    if (!resposta.ok) {
        throw new Error(`Erro HTTP: ${resposta.status}`);
    }

    dados = await resposta.json();
    console.log("Dados recebidos do Flask:", dados);

    // Adapta os nomes dos campos caso o Flask
    // retorne os nomes originais das colunas do MySQL.
    if (dados && typeof dados === "object" && !Array.isArray(dados)) {
        dados.pressão ??= dados.pressao;
        dados.gás ??= dados.qualidade_ar;

        if (!dados.Historico_de_Dados) {
            dados.Historico_de_Dados = dados.historico ?? [];
        }

        if (!dados.Nome_Estacao) {
            dados.Nome_Estacao = dados.nome_estacao ?? "ClimaSys";
        }

        if (dados.Historico_de_Dados.length > 0) {
            const Ultimo = dados.Historico_de_Dados[
                dados.Historico_de_Dados.length - 1
            ];

            dados.temperatura ??= Ultimo.temperatura;
            dados.umidade ??= Ultimo.umidade;
            dados.pressão ??= Ultimo.pressao ?? Ultimo.pressão;
            dados.luminosidade ??= Ultimo.luminosidade;
            dados.gás ??= Ultimo.qualidade_ar ?? Ultimo.gás;
            dados.Data_Hora ??= Ultimo.data_hora ?? Ultimo.created_at;
        }
    }

    return dados;
}

function Criar_Relatorio() {
    const exportBtn = Array.from(document.querySelectorAll("button"))
        .find(btn => btn.textContent.includes("Gerar Relatório CSV"));

    if (exportBtn && !exportBtn.dataset.csvListener) {
        // Evita registrar o evento duas vezes.
        exportBtn.dataset.csvListener = "true";

        exportBtn.addEventListener("click", (e) => {
            e.preventDefault();

            if (!dados || !Ultimo_Dado) {
                console.warn("Nenhum dado disponível para exportar.");
                return;
            }

            const reportData = [
                ["Data", "Estacao", "Temperatura (C)", "Umidade (%)", "Pressão do Ar", "Luminosidade", "Status"],
                [
                    Ultimo_Dado.data_hora ?? Ultimo_Dado.Data_Hora ?? "--",
                    dados.Nome_Estacao,
                    Ultimo_Dado.temperatura ?? "--",
                    Ultimo_Dado.umidade ?? "--",
                    Ultimo_Dado.pressao ?? Ultimo_Dado.pressão ?? "--",
                    Ultimo_Dado.luminosidade ?? "--",
                    dados.Codigo_HTTP ?? "--"
                ]
            ];

            // Protege valores com vírgulas e aspas.
            const csvContent = "\uFEFF" + reportData
                .map(linha => linha.map(valor =>
                    `"${String(valor ?? "--").replace(/"/g, '""')}"`
                ).join(";"))
                .join("\r\n");

            const arquivo = new Blob([csvContent], {
                type: "text/csv;charset=utf-8;"
            });

            const link = document.createElement("a");
            const URL_Arquivo = URL.createObjectURL(arquivo);

            link.href = URL_Arquivo;
            link.download = `relatorio_climatico_${new Date().toISOString().slice(0, 10)}.csv`;

            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
            URL.revokeObjectURL(URL_Arquivo);
        });
    }
}

function Atualizar_Recebimento(dados) {
    if (dados.Historico_de_Dados && dados.Historico_de_Dados.length > 0) {
        Pegar_Elemento_Por_ID("Recent_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Recent_Station_Data", "Enviou novos dados.", "");
        Pegar_Elemento_Por_ID(
            "Recent_Station_Time",
            dados.Data_Hora ?? dados.data_hora ?? "--",
            ""
        );
    } else {
        Pegar_Elemento_Por_ID("Recent_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Recent_Station_Data", "Sem dados.", "");
        Pegar_Elemento_Por_ID("Recent_Station_Time", "Sem atualização.", "");
    }
}

function Atualizar_Analise(dados) {
    if (dados.Historico_de_Dados && dados.Historico_de_Dados.length > 0) {
        Pegar_Elemento_Por_ID("Analytics_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Analytics_Station_Data", "Enviou novos dados.", "");
        Pegar_Elemento_Por_ID("Analytics_Updates_Value", dados.Qtd_Atualizados ?? dados.Historico_de_Dados.length, "");
    } else {
        Pegar_Elemento_Por_ID("Analytics_Station_Name", dados.Nome_Estacao, "");
        Pegar_Elemento_Por_ID("Analytics_Station_Data", "Sem dados.");
        Pegar_Elemento_Por_ID("Analytics_Updates_Value", dados.Qtd_Atualizados ?? 0, "");
        Pegar_Elemento_Por_ID("Analytics_Time", "Sem atualização.", "");
    }
}

function Atualizar_Tabela_de_Historicos(dados) {
    console.log("ATUALIZAR TABELAS");
    console.log("Histórico:", dados.Historico_de_Dados);

    Registro_do_Historico = dados.Historico_de_Dados ?? [];

    let Tabela_Historico_de_Dados = Registro_do_Historico;
    let Tamanho_Total = Tabela_Historico_de_Dados.length - 1;

    let tbody = document.querySelector(".recent-orders tbody");

    if (!tbody) {
        tbody = document.querySelector(".table-card tbody");
    }

    // Verifica o tbody antes de usá-lo e limpa as linhas anteriores para não duplicar os registros.
    if (!tbody) {
        console.error("Tabela não encontrada.");
        return;
    }

    tbody.innerHTML = "";

    if (Tabela_Historico_de_Dados.length === 0) {
        let tr = document.createElement("tr");
        tr.innerHTML = `<td colspan="4">Nenhum registro encontrado.</td>`;
        tbody.appendChild(tr);
    } else {
        Looping_Registros(
            Tamanho_Total,
            tbody.closest(".recent-orders") ? 10 : 20,
            0,
            tbody,
            Tabela_Historico_de_Dados
        );
    }

    console.log(tbody);
}

function Looping_Registros(Tamanho_Total, Limite_Repeticoes, Contador_Registros, tbody, Tabela_Historico_de_Dados) {
    while (
        Limite_Repeticoes > Contador_Registros &&
        Tamanho_Total >= 0
    ) {
        const Registro = Tabela_Historico_de_Dados[Tamanho_Total];

        // Utiliza o registro recebido, não um índice que possa estar desatualizado.
        const Data_Registro = Registro.data_hora ?? Registro.Data_Hora ?? Registro.created_at;
        const Data = Data_Registro ? new Date(Data_Registro) : null;
        const data_formatada = Data && !isNaN(Data.getTime())
            ? Data.toLocaleString("pt-BR")
            : "--";

        let tr = document.createElement("tr");

        tr.innerHTML = `
            <td>${dados.Nome_Estacao ?? "--"}</td>
            <td>${Registro.Id_Estacao ?? "--"}</td>
            <td>${data_formatada}</td>
            <td class="success">${dados.Codigo_HTTP ?? "200 OK"}</td>
        `;

        tbody.appendChild(tr);

        Tamanho_Total--;
        Contador_Registros++;
    }

    Contador_Registros = Contador_Registros;
}

function Pegar_Elemento_Por_ID(ID, Valor_Preencher, Sinal) {
    const Elemento_HTML = document.getElementById(ID);

    if (!Elemento_HTML) {
        console.error("Elemento não encontrado:", ID);
        return;
    }

    Elemento_HTML.textContent =
        `${Valor_Preencher ?? "--"} ${Sinal ?? ""}`.trim();
}

function Limpar_Tabela() {
    let tbody = document.querySelector(".recent-orders tbody");

    if (!tbody) {
        tbody = document.querySelector(".table-card tbody");
    }

    if (tbody) {
        tbody.innerHTML = "";
    }
}

function Limpar_Dashboard() {
    Limpar_Tabela();
    Pegar_Elemento_Por_ID("temperatura", "--", "°C");
    Pegar_Elemento_Por_ID("%_temperatura", "--", "%");
    Pegar_Elemento_Por_ID("umidade", "--", "%");
    Pegar_Elemento_Por_ID("%_umidade", "--", "%");
    Pegar_Elemento_Por_ID("pressão", "--", "hPa");
    Pegar_Elemento_Por_ID("%_pressão", "--", "%");
    Pegar_Elemento_Por_ID("luminosidade", "--", "");
    Pegar_Elemento_Por_ID("%_luminosidade", "--", "%");
    Pegar_Elemento_Por_ID("gás", "--", "");
    Pegar_Elemento_Por_ID("%_gas", "--", "%");

    Pegar_Elemento_Por_ID("Recent_Station_Name", "--", "");
    Pegar_Elemento_Por_ID("Recent_Station_Data", "Sem dados.", "");
    Pegar_Elemento_Por_ID("Recent_Station_Time", "Sem atualização.", "");
    Pegar_Elemento_Por_ID("Analytics_Station_Name", "--", "");
    Pegar_Elemento_Por_ID("Analytics_Station_Data", "Sem dados.", "");
    Pegar_Elemento_Por_ID("Analytics_Updates_Value", 0, "");
    Pegar_Elemento_Por_ID("Analytics_Time", "Sem atualização.", "");
}

function Atualizar_Progresso_Circulo(seletorClasse, valor, valorMaximo) {
    const circulo = document.querySelector(`.${seletorClasse} svg circle`);
    if (!circulo) return;

    const numero = Number(valor);
    const maximo = Number(valorMaximo);

    if (
        valor === null ||
        valor === undefined ||
        valor === "" ||
        !Number.isFinite(numero) ||
        !Number.isFinite(maximo) ||
        maximo <= 0
    ) {
        circulo.style.strokeDashoffset = "226";
        return;
    }

    const porcentagem = Math.min(Math.max((numero / maximo) * 100, 0), 100);
    const raio = Number(circulo.getAttribute("r"));
    const circunferencia = 2 * Math.PI * raio;

    circulo.style.strokeDasharray = circunferencia;
    circulo.style.strokeDashoffset = circunferencia - (circunferencia * porcentagem) / 100;
}

function Converter_Temperatura(valorCelsius) {
    if (
        valorCelsius === null ||
        valorCelsius === undefined ||
        valorCelsius === "" ||
        !Number.isFinite(Number(valorCelsius))
    ) {
        return { valor: "--", sinal: "°C" };
    }

    const unidadeGuardada = localStorage.getItem("pref_temp_unit");

    if (unidadeGuardada === "Fahrenheit (°F)") {
        const fahrenheit = (Number(valorCelsius) * 9 / 5) + 32;

        return {
            valor: fahrenheit.toFixed(1),
            sinal: "°F"
        };
    }

    return {
        valor: valorCelsius,
        sinal: "°C"
    };
}

function Agrupar_Elementos(dados) {
    if (!dados) return;

    if (!Pausar_Atualização) {
        Atualizar_Recebimento(dados);
        Atualizar_Analise(dados);
    }

    const tempConvertida = Converter_Temperatura(dados.temperatura);

    let pctTemp = dados.temperatura != null ? Math.min(Number(dados.temperatura) || 0, 100) : 0;
    let pctUmid = Number(dados.umidade) || 0;
    let pctPressao = dados.pressão != null ? (Number(dados.pressão) / 1100) * 100 : 0;
    let pctLuz = Number(dados.luminosidade) || 0;
    let pctGas = Number(dados.gás) || 0;

    Pegar_Elemento_Por_ID("temperatura", tempConvertida.valor, tempConvertida.sinal);
    Pegar_Elemento_Por_ID("%_temperatura", Math.round(pctTemp), "%");

    Pegar_Elemento_Por_ID("umidade", dados.umidade, "%");
    Pegar_Elemento_Por_ID("%_umidade", Math.round(pctUmid), "%");

    Pegar_Elemento_Por_ID("pressão", dados.pressão, "hPa");
    Pegar_Elemento_Por_ID("%_pressão", Math.round(pctPressao), "%");

    Pegar_Elemento_Por_ID("luminosidade", dados.luminosidade, "");
    Pegar_Elemento_Por_ID("%_luminosidade", Math.round(pctLuz), "%");

    Pegar_Elemento_Por_ID("gás", dados.gás, "");
    Pegar_Elemento_Por_ID("%_gas", Math.round(pctGas), "%");

    Atualizar_Progresso_Circulo("temperature", pctTemp, 50);
    Atualizar_Progresso_Circulo("humidity", pctUmid, 100);
    Atualizar_Progresso_Circulo("windspeed", pctPressao, 100);
    Atualizar_Progresso_Circulo("luz", pctLuz, 5000);
    Atualizar_Progresso_Circulo("Gás", pctGas, 100);

    console.log("ELEMENTOS E TEMPERATURA ATUALIZADOS");
}

async function Carregar_Primeira_Vez() {
    try {
        const Dados_Recebidos = await Buscar_Dados();

        Agrupar_Elementos(Dados_Recebidos);
        Atualizar_Tabela_de_Historicos(Dados_Recebidos);

        Ultimo_Dado = Registro_do_Historico.at(-1) ?? null;

        console.log("CARREGOU");
    } catch (erro) {
        console.error("Erro ao carregar:", erro);
    }
}

async function Atualizar_Dashboard() {
    // Não recebe argumentos antigos. Usa a resposta atual da API.
    try {
        if (Pausar_Atualização) return;

        const Dados_Recebidos = await Buscar_Dados();

        if (Dados_Recebidos.Atualizacao || Dados_Recebidos.Historico_de_Dados?.length) {
            Agrupar_Elementos(Dados_Recebidos);
            Atualizar_Tabela_de_Historicos(Dados_Recebidos);

            Ultimo_Dado = Registro_do_Historico.at(-1) ?? null;
        } else {
            console.log("Nenhuma atualização.");
        }
    } catch (erro) {
        console.error("Erro ao atualizar:", erro);
    }
}

async function Filtrar_por_Data() {
    const Input_Data =
        document.getElementById("Date_Filter") ??
        document.querySelector('input[type="date"]');

    if (!Input_Data) {
        console.error("Campo de data não encontrado.");
        return;
    }

    const Data_Selecionada = Input_Data.value;

    // Ao limpar a data, retorna à atualização normal.
    if (!Data_Selecionada) {
        Pausar_Atualização = false;
        await Carregar_Primeira_Vez();
        return;
    }

    Pausar_Atualização = true;

    try {
        const Resposta_Filtro = await Retornar_Dados_ao_Back(
            Data_Selecionada,
            "data"
        );

        const dados_filtrados = await Resposta_Filtro.json();

        // O Flask retorna uma lista de registros do MySQL.
        if (!Array.isArray(dados_filtrados)) {
            console.error("Resposta inesperada do Flask:", dados_filtrados);
            return;
        }

        Limpar_Dashboard();

        if (dados_filtrados.length === 0) {
            Registro_do_Historico = [];
            Ultimo_Dado = null;

            Atualizar_Tabela_de_Historicos({
                Nome_Estacao: dados?.Nome_Estacao ?? "ClimaSys",
                Historico_de_Dados: []
            });

            Pegar_Elemento_Por_ID(
                "Recent_Station_Data",
                "Nenhum registro nessa data.",
                ""
            );

            return;
        }

        // Adapta a lista filtrada ao formato esperado pelas funções existentes do dashboard.
        const Historico_Filtrado = dados_filtrados.map(Registro => ({
            ...Registro,
            pressão: Registro.pressão ?? Registro.pressao ?? null,
            gás: Registro.gás ?? Registro.qualidade_ar ?? null
        }));

        const Ultimo_Registro = Historico_Filtrado.at(-1);
        Ultimo_Dado = Ultimo_Registro;

        const Dados_Dashboard = {
            Nome_Estacao: dados?.Nome_Estacao ?? "ClimaSys",
            temperatura: Ultimo_Registro.temperatura ?? null,
            umidade: Ultimo_Registro.umidade ?? null,
            pressão: Ultimo_Registro.pressão,
            luminosidade: Ultimo_Registro.luminosidade ?? null,
            gás: Ultimo_Registro.gás,
            Codigo_HTTP: "200 OK",
            Qtd_Atualizados: Historico_Filtrado.length,
            Atualizacao: true,
            Data_Hora: Ultimo_Registro.data_hora ?? null,
            Historico_de_Dados: Historico_Filtrado
        };

        // Permite atualizar os indicadores mesmo durante o filtro.
        Agrupar_Elementos(Dados_Dashboard);
        Atualizar_Tabela_de_Historicos(Dados_Dashboard);

        console.log("Dados filtrados:", Historico_Filtrado);
    } catch (erro) {
        console.error("ERRO NO FILTRO:", erro);
    } finally {
        Pausar_Atualização = false;
    }
}

async function Iniciar_Programa() {
    await Carregar_Primeira_Vez();

    Criar_Relatorio();

    setInterval(() => {
        if (!Pausar_Atualização) {
            Atualizar_Dashboard();
        }
    }, 10000);
}

Iniciar_Programa();
```

</details>
<details>
<summary> Mapa.js </summary>

```csharp
const RENDER_URL = "https://projetos-estacao-meteorol-gica.onrender.com/dados";
let dados;

// Puxa os dados da API para cá.
async function Buscar_Dados() {
    const resposta = await fetch(RENDER_URL);
    if (!resposta.ok) {
        throw new Error(`Erro HTTP: ${resposta.status}`);
    }

    dados = await resposta.json();
    console.log(dados);
    return dados;
}

// Cria o mapa somente após receber os dados da API (com a função Buscar_Dados() ). Depois, aplica a longitude e latitude, nome e temperatura recebidos.
const mapElement = document.getElementById('map');
if (mapElement && typeof L !== 'undefined') {
    const map = L.map('map').setView([-23.4735, -46.7231], 13);
    L.tileLayer(
        'https://server.arcgisonline.com/ArcGIS/rest/services/World_Street_Map/MapServer/tile/{z}/{y}/{x}',
        {
            attribution: 'Tiles &copy; Esri'
        }
    ).addTo(map);

    // Espera os dados da API
    Buscar_Dados()
        .then(dados => {
            const station = {
                name: dados.Nome_Estacao ?? "Estação sem nome",
                status: "Online",
                temp: dados.temperatura ?? "--",
                lat: Number(dados.latitude),
                lng: Number(dados.longitude)
            };
            //verificação das coordenadas
            if (isNaN(station.lat) || isNaN(station.lng)) {
                console.error("Coordenadas inválidas:", station);
                return;
            }
            L.marker([station.lat, station.lng])
                .addTo(map)
                .bindPopup(`
                    <b>${station.name}</b><br>
                    Status: ${station.status}<br>
                    Temp: ${station.temp} °C
                `);
        })
        .catch(erro => {
            console.error("Erro ao carregar dados da estação:", erro);
        });

    setTimeout(() => {
        map.invalidateSize();
    }, 300);
}
```

</details>
<details>
<summary> Preferencias.js </summary>

```csharp
    // Busca os elementos de "Query" no html da página. Inclusive, adiciona um texto ao botão que, no contexto da página, serve para salvar as preferências
    const tempUnitSelect = document.querySelector('.settings-form select');
    const emailCheckbox = document.querySelector('.settings-form input[type="checkbox"]');
    const saveSettingsBtn = Array.from(document.querySelectorAll('button')).find(btn => btn.textContent.includes('Salvar Alterações'));

    // Caso os itens existam, ele pega os valores de preferência e, ao salvar e confirmar, armazena os valores escolhidos pelo usuário
    if (tempUnitSelect && emailCheckbox) {
        const savedUnit = localStorage.getItem('pref_temp_unit');
        const savedEmailNotif = localStorage.getItem('pref_email_notif');

        if (savedUnit) tempUnitSelect.value = savedUnit;
        if (savedEmailNotif !== null) emailCheckbox.checked = JSON.parse(savedEmailNotif);
    }

    if (saveSettingsBtn) {
        saveSettingsBtn.addEventListener('click', (e) => {
            e.preventDefault();

            if (tempUnitSelect && emailCheckbox) {
                localStorage.setItem('pref_temp_unit', tempUnitSelect.value);
                localStorage.setItem('pref_email_notif', emailCheckbox.checked);

                alert('Preferências salvas com sucesso!');
            }
        });
    }
```

</details>
</details>


</details>
