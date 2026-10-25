>[!Important]
 > `Repositório - Projetos`
>- Turma: 2° Semestre de Ciência da Computação.
>- Faculdade: Universidade Paulista.
>- Polo: UNIP Marquês.
>- Sobre: Repositório para a documentação do projeto de Estação Metereológica do 2° Semestre.
>- Membros: Alex Campos de Oliveira, Rafael Arruda, Rafael Alamino, Rafael Torso.

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


</details>

<details>
<summary> configuracoes.html </summary>


</details>

<details>
<summary> ingestao.html </summary>


</details>


<details>
<summary> mapa.html </summary>


</details>

<details>
<summary> CSS </summary>
 
</details>
</details>

<details>
<summary> CSS </summary>
<details>
<summary> style.css </summary>


</details>


</details>

<details>
<summary> SQL </summary>


</details>

<details>
<summary> Back-End </summary>
 <details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
</details>

<details>
<summary> Front-End </summary>
<details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
<details>
<summary> ingestao.html </summary>


</details>
</details>


</details>
